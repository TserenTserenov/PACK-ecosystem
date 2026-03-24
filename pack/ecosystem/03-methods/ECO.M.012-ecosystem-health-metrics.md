---
id: ECO.M.012
title: "Ecosystem Health Metrics"
type: method
status: active
created: 2026-03-24
source: "Bevy Community Metrics 2025, Innoloft Engagement Metrics, ASAE Community Success, Thinkific Community Metrics, Disco Community Insights, GlueUp Engagement"
related: [ECO.M.010, ECO.M.013, ECO.SOTA.005]
s2r_families: [F6]
---

# ECO.M.012: Ecosystem Health Metrics

> **Назначение:** Метод измерения здоровья экосистемы — не только продукта (F2), но всей системы взаимодействий между участниками.

---

## 1. Определение

Ecosystem Health — состояние экосистемы, при котором участники создают ценность друг для друга, новые участники присоединяются, а существующие остаются и углубляют участие.

**Различение:** Ecosystem Health ≠ Product Metrics. Product metrics (F2) измеряют продукт глазами пользователя. Ecosystem health измеряет *систему взаимодействий* — включая peer-to-peer ценность, partner engagement, content generation.

**SOTA 2025:** Vanity metrics (likes, followers) уступают depth metrics: authentic interactions, sustained participation, real-time sentiment.

---

## 2. Четыре измерения здоровья

| Измерение | Вопрос | Ключевые метрики |
|-----------|--------|-----------------|
| **Engagement** | Участвуют ли активно? | DAU/MAU, session depth, interaction rate |
| **Growth** | Растёт ли экосистема? | New member rate, net growth, referral rate |
| **Retention** | Остаются ли? | 30/60/90-day retention по когортам |
| **Contribution** | Создают ли ценность друг для друга? | UGC ratio, peer-to-peer %, answer rate |

---

## 3. Метрики по измерениям

### Engagement

| Метрика | Формула | Healthy benchmark |
|---------|---------|-------------------|
| Active Member Rate | Active / Total members | >20% |
| Interaction Depth | Actions per active member per week | >3 |
| Content Interaction Rate | Members who interact with content / Active | >30% |
| Event Participation Rate | Attendees / Invited | >15% |

### Growth

| Метрика | Формула | Healthy benchmark |
|---------|---------|-------------------|
| Net Member Growth | (New - Churned) / Total | >5% monthly |
| Organic Acquisition % | Organic new / Total new | >30% |
| Referral Rate | Members who invited / Active | >10% |
| Time to First Value | Signup → first meaningful action | <24h |

### Retention (когортный анализ)

| Метрика | Формула | Healthy benchmark |
|---------|---------|-------------------|
| D30 Retention | Active at Day 30 / Cohort size | >25% (community) |
| D90 Retention | Active at Day 90 / Cohort size | >15% |
| Reactivation Rate | Returned inactive / Total inactive | >5% monthly |
| Churn Reason | Top 3 reasons by exit survey | Track quarterly |

### Contribution (самый важный для экосистемы)

| Метрика | Формула | Healthy benchmark |
|---------|---------|-------------------|
| UGC Ratio | User-generated content / Total content | >30% |
| Peer-to-Peer % | Peer answers / Total answers | >50% |
| Creator to Consumer | Members who create / Members who consume | >1:9 (1% rule) → target >1:5 |
| Knowledge Sharing Index | Shared resources / Active members | >0.5/мес |

---

## 4. Ecosystem Health Score (композитный)

| Измерение | Вес | Максимум |
|-----------|-----|----------|
| Engagement | 25% | 25 |
| Growth | 20% | 20 |
| Retention | 30% | 30 |
| Contribution | 25% | 25 |
| **Итого** | **100%** | **100** |

**Интерпретация:**
- 0-30: Кризис. Экосистема не самоподдерживается.
- 31-50: Уязвимость. Зависит от core team efforts.
- 51-70: Здоровая. Есть organic activity.
- 71-100: Процветающая. Self-sustaining с сетевыми эффектами.

---

## 5. Early Warning Signals (красные флаги)

| Сигнал | Что означает | Порог |
|--------|-------------|-------|
| Падение peer-to-peer % | Сообщество «умирает», модераторы тянут | <30% и падает |
| Рост inactive members | Зарегистрировались, но не участвуют | >60% inactive |
| Снижение UGC | Контент генерирует только команда | UGC <10% |
| Рост churn без роста new | Экосистема сжимается | Net growth <0 два месяца |
| Снижение event attendance | Потеря интереса к live interaction | <10% attendance |

---

## 6. Применение к IWE

| Измерение | Что измерять | Источник данных |
|-----------|-------------|----------------|
| **Engagement** | Активность в Клубе, взаимодействие с ботом | Discourse API, bot analytics |
| **Growth** | Новые участники, источник привлечения | LMS, referral tracking |
| **Retention** | Когортный анализ по курсам и клубу | Neon DB, Digital Twin |
| **Contribution** | Посты в клубе от участников, менторство | Discourse API |

---

## 7. Failure modes

| ID | Ошибка | Последствие |
|----|--------|-------------|
| FM.EH.001 | Измерять только vanity metrics (followers, likes) | Ложное чувство здоровья |
| FM.EH.002 | Не отслеживать contribution | Не видим, что community умирает |
| FM.EH.003 | Игнорировать cohort analysis | Средние скрывают ухудшение |
| FM.EH.004 | Реагировать на метрики, не на причины | Симптоматическое лечение |
| FM.EH.005 | Один dashboard для всех | Разные стейкхолдеры нуждаются в разных метриках |
