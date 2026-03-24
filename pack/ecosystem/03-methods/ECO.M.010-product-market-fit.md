---
id: ECO.M.010
title: "Product-Market Fit Measurement"
type: method
status: active
created: 2026-03-24
source: "PM Toolkit PMF Guide, Mag Startup PMF 2026, Qubit Capital PMF Framework, WeArePresta PMF 2026, Pisano Sean Ellis Test"
related: [ECO.M.006, ECO.M.011, ECO.SOTA.005]
s2r_families: [F2]
---

# ECO.M.010: Product-Market Fit Measurement

> **Назначение:** Метод измерения и валидации product-market fit (PMF) — ключевого перехода от «строим» к «масштабируем».

---

## 1. Определение

Product-Market Fit — состояние, при котором продукт решает реальную проблему для определённого сегмента настолько хорошо, что пользователи не хотят от него отказываться и рекомендуют другим.

**Различение:** PMF ≠ product launch. PMF ≠ первые платящие клиенты. PMF = измеримое доказательство, что пользователи *нуждаются* в продукте.

---

## 2. Пять сигналов PMF (Multi-Signal Framework)

> Ни один метрик в одиночку не подтверждает PMF. Нужна конвергенция 3+ сигналов.

| # | Сигнал | Метод измерения | Порог «есть PMF» |
|---|--------|----------------|-------------------|
| 1 | **Sean Ellis Test** | Опрос: «Что бы вы почувствовали, если бы не могли больше использовать [продукт]?» | ≥40% «very disappointed» |
| 2 | **Cohort Retention** | D30 retention по когортам | ≥40% (high-frequency), ≥20% (low-frequency) |
| 3 | **NPS** | Net Promoter Score | >50 |
| 4 | **CAC Payback** | Полные затраты на привлечение / gross margin | <12 мес (B2B), <6 мес (B2C) |
| 5 | **Organic Growth** | % новых пользователей из organic/referral | >30% organic |

### Приоритет сигналов

**Sean Ellis Test — фундамент.** Если <25%, PMF score cap = 50 (даже если остальные метрики хорошие). Это значит: ядро ценности не найдено.

---

## 3. Sean Ellis Test: протокол

1. **Когда проводить:** После 7-14 дней использования (не в первый день)
2. **Минимум респондентов:** 40
3. **Вопрос:** «Как бы вы себя почувствовали, если бы больше не могли использовать [продукт]?»
4. **Варианты:** Very disappointed / Somewhat disappointed / Not disappointed / N/A
5. **Расчёт:** % «very disappointed» от (total - N/A)
6. **Периодичность:** Ежеквартально

### Follow-up вопросы (для диагностики)

- «В чём основная ценность [продукта] для вас?» → Core value proposition
- «Кому бы вы порекомендовали [продукт]?» → Целевой сегмент глазами пользователя
- «Как бы вы улучшили [продукт]?» → Направление развития

---

## 4. Cohort Retention Analysis

| Метрика | Формула | Benchmark EdTech |
|---------|---------|-----------------|
| D1 retention | Users active Day 1 / Signups | 40-60% |
| D7 retention | Users active Day 7 / Signups | 20-35% |
| D30 retention | Users active Day 30 / Signups | 10-25% |
| M3 retention | Users active Month 3 / Signups | 5-15% |

**Ключевое:** Смотреть не средние, а **форму кривой**. PMF = кривая выходит на плато (не падает к нулю).

### Retention по типу EdTech

| Тип | D30 benchmark | Причина |
|-----|--------------|---------|
| Language learning (Duolingo) | 35-45% | Ежедневная привычка |
| Professional upskilling | 15-25% | Еженедельное использование |
| Course platform (LMS) | 8-15% | Периодическое (по курсу) |
| Community/club | 20-30% | Зависит от social engagement |

---

## 5. PMF Score Calculator

Взвешенная формула из 5 сигналов:

| Сигнал | Вес | Максимум |
|--------|-----|----------|
| Sean Ellis | 30% | 30 |
| Retention | 25% | 25 |
| NPS | 20% | 20 |
| CAC Payback | 15% | 15 |
| Organic Growth | 10% | 10 |
| **Итого** | **100%** | **100** |

**Интерпретация:**
- 0-30: Нет PMF. Пивот или радикальное изменение.
- 31-50: Ранние сигналы. Найти ядро ценности.
- 51-70: Есть PMF для узкого сегмента. Углублять.
- 71-100: Сильный PMF. Масштабировать.

---

## 6. Применение к IWE

| Сигнал | Текущее | Целевое |
|--------|---------|---------|
| Sean Ellis | Не измерялся | Внедрить в бот/LMS после 14 дней |
| D30 Retention | Есть данные по LMS | Добавить когортный анализ |
| NPS | Не измерялся | NPS-опрос через бота ежеквартально |
| CAC Payback | Community-led (CAC ≈ 0) | Трекать при масштабировании |
| Organic Growth | Высокий (word of mouth) | Формализовать referral tracking |

---

## 7. Failure modes

| ID | Ошибка | Последствие |
|----|--------|-------------|
| FM.PMF.001 | Масштабировать до PMF | Burn cash на growth без retention |
| FM.PMF.002 | Одна метрика как proof of PMF | Ложная уверенность (высокий NPS, но 5% retention) |
| FM.PMF.003 | Sean Ellis после 1 дня | Неинформативно — пользователь не успел получить ценность |
| FM.PMF.004 | Опрашивать только power users | Selection bias — PMF для ядра, но не для рынка |
| FM.PMF.005 | Игнорировать сегментацию | PMF может быть для одного сегмента, но не для другого |
