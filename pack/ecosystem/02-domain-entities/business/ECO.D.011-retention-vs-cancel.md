---
id: ECO.D.011
name: "Retention-сигнал ≠ Cancel"
type: distinction
status: draft
trust: draft
epistemic_stage: initial
source_wp: WP-377
valid_from: 2026-05-31
s2r_families: [F7]
related:
  see_also:
    - "DP.SC.121 (PII boundaries)"
    - "DP.SC.112 (Подписка и оплата)"
    - "ECO.D.010 (подписка ≠ покупка ≠ донат)"
    - "ECO.D.012 (возмездная транзакция ≠ учёт балансов)"
---

# ECO.D.011: Retention-сигнал ≠ Cancel

## Различение

Два разных типа сигналов о статусе плательщика в подписочной модели. Смешение приводит к ложным churn-метрикам и неверной интерпретации поведения.

| Класс | Природа сигнала | Источник | Действие со стороны плательщика |
|-------|----------------|----------|--------------------------------|
| **Retention-сигнал** | Активность (или продление платежа) за период | Бот, платформа, биллинг | НЕ требуется явное действие — авто-renew или просто использование |
| **Cancel** | Явный отказ от продолжения отношения | Кнопка «отписаться», банк отозвал транзакцию, чат-боту команда `/cancel` | Требуется явное действие плательщика или системы (chargeback) |

**Retention-сигнал** — производный показатель: «человек продолжает быть в системе». Складывается из:
- последняя сессия в боте / приложении не далее N дней,
- объём использования продукта (просмотры, действия, slot_logged),
- факт продления платежа в текущем billing-цикле.

**Cancel** — атомарное событие: «отношения прекращены». Имеет timestamp и причину (user-initiated, payment-failed, fraud, gdpr-erasure и др.).

## Тесты различения

1. **«Может ли пользователь быть retained без явного действия?»** Да — auto-renew подписки + редкие визиты по-прежнему считаются retention.
2. **«Может ли пользователь быть cancelled без сигнала pre-cancel?»** Да — silent churn (банк отозвал карту, истёк срок без продления при отсутствии auto-renew, технический сбой биллинг-системы).
3. **«Можно ли восстановить retention постфактум по логам?»** Да — retention — derived-метрика из activity_log. Cancel — событие с timestamp, нельзя «вычислить» из активности.

## GDPR-нота

> Retention-данные хранятся согласно [DP.SC.121](../../../../../PACK-digital-platform/pack/digital-platform/08-service-clauses/DP.SC.121-ontology-grounded-answers.md) (PII boundaries).
>
> При обработке `right-to-be-forgotten` запроса (B-004 в backlog) **retention-history субъекта удаляется одновременно с PII**: события `activity_log`, payment-history с привязкой к ory_id, любые derived-агрегаты на per-user уровне.
>
> Кэши и derived-метрики **по когортам** (агрегаты W{N}-cohort retention, MRR/ARR по сегментам без user-привязки) сохраняются только в обезличенном виде — без возможности восстановить identity субъекта.
>
> Cancel-события с причиной `gdpr-erasure` фиксируются с metadata, достаточной для аудита факта удаления, но без PII.

## Соседи (НЕ путать)

- **Churn** = доля cancel-событий в когорте за период. Метрика, не сигнал.
- **Inactive** ≠ cancel. Inactive — отсутствие retention-сигнала, но без явного cancel. Может перейти в churn по правилу (например, 90 дней inactive → принудительный downgrade).
- **Pause / Suspend** — приостановка подписки. Не cancel (отношение сохранено), не retention (биллинг приостановлен). Отдельный класс.

## Применимость

Используется при:
- проектировании метрик MRR/ARR/churn (когда суммировать, когда исключать),
- настройке retention-уведомлений (только по retention-сигналам, не по cancel),
- обработке GDPR-запросов (что удалять, что обезличивать),
- разделении silent churn vs voluntary churn в отчётах для пилота.

## Связь

- [ECO.D.010](ECO.D.010-payment-models.md) — подписка ≠ покупка ≠ донат (контекст применимости: retention/cancel релевантны подписке).
- [ECO.D.012](ECO.D.012-money-vs-balances.md) — возмездная транзакция ≠ учёт балансов.
- [DP.SC.121](../../../../../PACK-digital-platform/pack/digital-platform/08-service-clauses/DP.SC.121-ontology-grounded-answers.md) — PII boundaries.
- [DP.SC.112](../../../../../PACK-digital-platform/pack/digital-platform/08-service-clauses/DP.SC.112-subscription-billing.md) — реализация cancel-flow на платформе (grace 7 дней).
