# Business sub-domain (v1 mini)

> **Мини-инкарнация v1** под-домена «бизнес» внутри PACK-ecosystem. Создана в Ф1.3' WP-377 (Variant C из CONSENSUS peer-сессии 2026-05-31-18).
>
> **Назначение:** дать онтологическую опору 5 активным платёжным РП (WP-231, WP-238, WP-246, WP-266) без преждевременного спина полного PACK-business. Терминология ещё кристаллизуется; LTV/ARPU/cohort-аналитика требуют GDPR-механизма account-deletion (B-004 в backlog) — поэтому в v1 не входят.

## Каталог артефактов

| ID | Тип | Назв. | Файл |
|----|-----|-------|------|
| **ECO.D.010** | Distinction | Подписка ≠ Покупка ≠ Донат | [ECO.D.010-payment-models.md](ECO.D.010-payment-models.md) |
| **ECO.D.011** | Distinction | Retention-сигнал ≠ Cancel | [ECO.D.011-retention-vs-cancel.md](ECO.D.011-retention-vs-cancel.md) |
| **ECO.D.012** | Distinction | Возмездная транзакция ≠ Учёт балансов | [ECO.D.012-money-vs-balances.md](ECO.D.012-money-vs-balances.md) |
| **ECO.SC.001** | Service Clause | Деньги поступили на счёт за N банковских дней | [ECO.SC.001-payment-receipt.md](ECO.SC.001-payment-receipt.md) |
| **ECO.SC.002** | Service Clause | Возврат за X (полный или частичный) | [ECO.SC.002-refund-policy.md](ECO.SC.002-refund-policy.md) |

## Что НЕ входит в v1 (отложено в v2)

- **LTV / ARPU / cohort-аналитика** — требует механизма account-deletion (B-004 GDPR).
- **Юнит-экономика по каналам** (CAC, payback period, contribution margin) — терминология ещё не устоялась.
- **Revenue Sharing деталь** — описан в DP.SC.112; полная онтология стейкхолдеров — v2.
- **Налоговая модель** — отдельный slice (юрисдикции, проводки, декларации).
- **Корпоративные подписки B2B-онтология** — описан flow в DP.SC.112 Путь C; полная модель контрактов — v2.

## Когда мигрировать в полный PACK-business v2

Триггеры:
1. Реализован B-004 (account-deletion с retention-history erasure → ECO.D.011 GDPR-нота снимается с «обещания» на «факт»).
2. Терминология LTV/ARPU/churn стабилизировалась в 5+ платёжных РП (нет дрифта в DS-репо).
3. Появляется ≥2 новых под-доменов (например, «налоговый учёт», «B2B-контракты») — нужно отделить от ECO.

При миграции: 5 артефактов этой папки переносятся как `BIZ.D.001-005` / `BIZ.SC.001-002` (или принятый префикс) в новый PACK-business; здесь — pointer-stub.

## Конвенция

- **Layer SC:** `L7-Business` (новый layer для бизнес-домена; не пересекается с L2-Platform / L4-Personal в DP).
- **Префикс:** `ECO.D.NNN` (D от 010) / `ECO.SC.NNN` (новый класс в PACK-ecosystem; первая нумерация).
- **s2r_families:** все артефакты v1 в `F7` (Бизнес — Предприниматель × Система-создания).

## Связь

- Upstream: PACK-ecosystem (этот Pack).
- Cross-Pack: PACK-digital-platform (`DP.SC.112` subscription-billing, `DP.SC.121` PII boundaries).
- Downstream: DS-ecosystem-development (5 платёжных РП: WP-231, WP-238, WP-246, WP-266).
