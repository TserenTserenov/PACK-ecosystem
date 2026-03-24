---
id: ECO.M.011
title: "Pricing Strategy (Freemium, Tiered, Usage-Based)"
type: method
status: active
created: 2026-03-24
source: "Monetizely EdTech Pricing, Revenera SaaS Pricing 2026, NxCode Pricing Guide 2026, Golden Door Software Pricing 2026, OpenFieldX EdTech Pricing"
related: [ECO.M.010, ECO.M.004, ECO.SOTA.002]
s2r_families: [F2]
---

# ECO.M.011: Pricing Strategy (Freemium, Tiered, Usage-Based)

> **Назначение:** Метод выбора и построения модели ценообразования для экосистемного продукта на стыке EdTech и AI.

---

## 1. Определение

Pricing strategy — стратегический выбор модели ценообразования, определяющий кто платит, за что, сколько и когда. В экосистеме pricing влияет не только на revenue, но и на adoption, network effects и ecosystem health.

**Различение:** Pricing ≠ Monetization. Pricing = конкретная модель (freemium, $X/мес). Monetization = общая стратегия создания revenue (включая pricing, upsell, cross-sell, data, marketplace commission).

---

## 2. Шесть моделей ценообразования (SaaS 2026)

| Модель | Суть | Когда работает | EdTech fit |
|--------|------|---------------|------------|
| **Freemium** | Бесплатный tier + платные features | B2C, mass adoption, viral loop | ⭐⭐⭐ (92% учителей пробуют через free) |
| **Tiered (3-4 уровня)** | Good/Better/Best packages | Разные сегменты, upgrade path | ⭐⭐⭐ (стандарт EdTech) |
| **Per-seat** | Цена × количество пользователей | B2B, teams, организации | ⭐⭐ (школы, университеты) |
| **Usage-based** | Pay per API call / active user | Developers, integrators | ⭐⭐ (Agent SDK, API access) |
| **Outcome-based** | Платишь за результат (job placement, skill gain) | Enterprise, high-trust | ⭐ (сложно измерить в education, cash flow gap, adverse selection risk. Тренд 2026: школьные округа USA тестируют outcome-based contracts) |
| **Hybrid** | Комбинация (subscription + usage) | Complex ecosystems | ⭐⭐⭐ (IWE target) |

---

## 3. Freemium: анатомия для EdTech

### Три линии разделения Free/Paid

| Линия | Как работает | Пример (IWE) |
|-------|-------------|---------------|
| **Feature-gated** | Core бесплатно, premium features платно | Курсы free → AI coaching paid |
| **Usage-gated** | Лимит использования | 5 вопросов к Digital Twin/день free → unlimited paid |
| **Time-gated** | Полный доступ на N дней | 14-day trial полного функционала |

### SOTA 2026: Freemium + AI upsell

AI-фичи размещаются в mid/upper tier для стимулирования upgrade:
- **Free:** Базовый контент, community доступ
- **Pro:** AI coaching, персонализация, Digital Twin
- **Enterprise:** API access, analytics, custom integrations

### Метрики Freemium

| Метрика | Benchmark EdTech |
|---------|-----------------|
| Free → Paid conversion | 2-5% (B2C), 10-15% (B2B) |
| Time to conversion | 30-90 дней |
| Free user LTV (через referral) | $5-15 |

---

## 4. Tiered Pricing: структура

### Правило «3 тiers + Enterprise»

| Tier | Цель | Ценовой якорь |
|------|------|---------------|
| **Free / Starter** | Привлечение, adoption | $0 |
| **Pro / Growth** | Основной revenue | Mid-market anchor |
| **Team / Business** | Организации | 2-3× Pro |
| **Enterprise** | Custom | По запросу |

### Value metrics (за что платят)

| Value metric | Кто платит | Пример |
|-------------|-----------|---------|
| Количество пользователей | Организации | Per-seat |
| Объём AI usage | Power users | Tokens / queries |
| Количество интеграций | Developers | API calls |
| Доступ к контенту | Индивидуальные | Courses / modules |

---

## 5. Процесс выбора модели

1. **Определить ICP** (Ideal Customer Profile) → кто основной плательщик?
2. **Определить value metric** → за что они готовы платить?
3. **Benchmarking** → что берут конкуренты за аналог?
4. **Willingness-to-pay research** → Van Westendorp или Gabor-Granger тест
5. **Tier design** → 3-4 пакета с чётким upgrade path
6. **Iterate** → A/B тестирование, ежеквартальный review

---

## 6. Применение к IWE

### Рекомендуемая модель: Hybrid (Freemium + Tiered + Usage)

| Tier | Цена | Включено |
|------|------|----------|
| **Free** | $0 | Вводные курсы, community (read-only), Digital Twin (лимит) |
| **Pro** | $X/мес | Все курсы, AI coaching, community (full), Digital Twin (unlimited) |
| **Team** | $Y/seat/мес | Pro + team analytics, shared workspaces |
| **API** | Usage-based | Agent SDK access, Digital Twin API, webhooks |

### EdTech-специфичные факторы

- **K-12:** Чувствительны к per-student pricing → flat rate per school предпочтительнее
- **Higher Ed:** Department-based licensing → per-seat с volume discount
- **Individual:** Подписка с годовой скидкой (20-30%) стандарт
- **Прозрачность:** Образовательные учреждения требуют predictable pricing для approval

---

## 7. Failure modes

| ID | Ошибка | Последствие |
|----|--------|-------------|
| FM.PR.001 | Слишком щедрый free tier | Нет мотивации upgrade, revenue = 0 |
| FM.PR.002 | Слишком жёсткий free tier | Нет adoption, никто не пробует |
| FM.PR.003 | Одна цена для всех | Потеря B2B (слишком дёшево) или B2C (слишком дорого) |
| FM.PR.004 | Менять цены без grandfathering | Churn существующих клиентов |
| FM.PR.005 | Pricing без WTP research | Цена из головы, а не от рынка |
| FM.PR.006 | Скрытые ограничения | Потеря доверия, negative reviews |
