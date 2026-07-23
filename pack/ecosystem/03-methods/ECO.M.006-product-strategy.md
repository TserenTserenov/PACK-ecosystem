---
id: ECO.M.006
title: "Стратегия продукта (Product Strategy)"
type: method
status: active
created: 2026-03-24
last_updated: 2026-07-23
source: "ProductSchool, ProductPlan, Ant Murphy, Product Compass"
related: [ECO.D.004, ECO.M.005, ECO.M.003]
s2r_families: [F4]
---

# ECO.M.006: Стратегия продукта (Product Strategy)

> **Назначение:** Метод формулирования стратегии продукта — мост между vision и roadmap.

---

## 1. Определение

Product Strategy — документ, определяющий:
1. **Кому** продаём (ICP — Ideal Customer Profile)
2. **Какую проблему** решаем (JTBD → ECO.M.003)
3. **Чем отличаемся** (moat / differentiation)
4. **Как зарабатываем** (business model)
5. **Как растём** (growth model: PLG, CLG, Sales-led)

**Различение:** Product Strategy ≠ Vision ≠ Roadmap (ECO.D.004).

---

## Forces

_(Optional, WP-448 Ф12) Какие конкурирующие давления удерживает метод._

| Force | Tension |
|-------|---------|
| Сила moat (§2.2: network effects «Сильнейший») ↔ скорость его построения | Сильнейшие moat (network effects, data moat) требуют больше времени на построение; более доступные moat (brand/community, «Средний») строятся быстрее, но защищают слабее |
| Growth Model под сегмент (§2.3: PLG/CLG/Sales-Led/Hybrid) ↔ операционная простота | Hybrid покрывает multi-segment, но требует «Blended CAC, segment-specific metrics» (больше сложности); единая модель проще в операциях, но рискует FM.PS.005 (одна модель для всех сегментов) |
| Стабильность Vision (§4: раз в 1-3 года) ↔ отзывчивость Strategy на новые данные (1-2 раза в год) | Стабильный канвас (§3) удобен для выравнивания команды, но частые обновления нужны, когда рынок/PMF меняются быстрее цикла — иначе FM.PS.004 (устаревшие допущения) |

---

## 2. Компоненты стратегии

### 2.1 ICP (Ideal Customer Profile)

| Атрибут | Описание |
|---------|----------|
| **Демография** | Возраст, роль, уровень опыта |
| **Контекст** | Чем занимается, какие инструменты использует |
| **Pain point** | Что болит (JTBD: функциональный, эмоциональный, социальный) |
| **Willingness to pay** | Сколько готов платить за решение |
| **Channels** | Где обитает (community, LinkedIn, conferences) |

### 2.2 Competitive Moat (защитное преимущество)

| Тип moat | Пример | Сила |
|----------|--------|------|
| **Network effects** | Больше пользователей → лучше AI → больше пользователей | Сильнейший |
| **Data moat** | Уникальные данные об обучении, Digital Twin | Сильный |
| **Switching cost** | Пользователь инвестировал время в систему | Средний |
| **Brand / Community** | Доверие сообщества, thought leadership | Средний |
| **Methodology** | Open methodology как Red Hat = open source | Уникальный для IWE |

### 2.3 Growth Model

| Модель | Когда | Метрика |
|--------|-------|---------|
| **PLG** | B2C, low ARPU (<$50/мес) | Activation rate, free-to-paid conversion |
| **CLG** | Expert products, strong community | Community engagement, referral rate |
| **Sales-Led** | B2B, high ACV (>$10K) | Pipeline velocity, win rate |
| **Hybrid** | Multi-segment (B2C + B2B) | Blended CAC, segment-specific metrics |

---

## 3. Product Strategy Canvas (шаблон)

```
┌─────────────────────────────────────────────┐
│ VISION: [1-2 предложения]                    │
├─────────────────────────────────────────────┤
│ ICP: Кто?          │ PROBLEM: Что болит?     │
├─────────────────────┼───────────────────────┤
│ SOLUTION: Что       │ MOAT: Почему мы?        │
│ делаем?             │                         │
├─────────────────────┼───────────────────────┤
│ BUSINESS MODEL:     │ GROWTH MODEL:           │
│ Как зарабатываем?   │ Как растём?             │
├─────────────────────┴───────────────────────┤
│ KEY METRICS: [3-5 метрик]                    │
│ RISKS: [top 3 риска]                         │
└─────────────────────────────────────────────┘
```

---

## 4. Cadence обновления

| Артефакт | Частота | Триггер |
|----------|---------|---------|
| Vision | Редко (раз в 1-3 года) | Фундаментальный сдвиг рынка |
| Strategy | 1-2 раза в год | Новые данные о PMF, pivot, новый сегмент |
| Roadmap | Ежеквартально | Market feedback, team capacity |

---

## 5. Failure modes

| ID | Ошибка | Последствие |
|----|--------|-------------|
| FM.PS.001 | Strategy = список фич | Feature factory без направления |
| FM.PS.002 | Нет ICP (продаём всем) | Распылённый messaging, высокий CAC |
| FM.PS.003 | Moat = «наша команда» | Не масштабируется, не защищает |
| FM.PS.004 | Strategy не обновляется | Год работаем по устаревшим допущениям |
| FM.PS.005 | Один growth model для всех сегментов | B2C не закрывается через sales, B2B не через PLG |

---

## Bias-Annotation

_(Optional, WP-448 Ф12) Куда систематически съезжает внимание практикующего. Не дублирует «Failure modes» — там «что пойдёт не так», здесь «куда дрейфует внимание»._

| Bias | Direction of distortion |
|------|--------------------------|
| ICP/Solution легче Moat | При заполнении Product Strategy Canvas (§3) внимание смещается к блокам ICP и Solution (легко описываются) и уходит от Moat («Почему мы?» — самый трудный блок для честной оценки), из-за чего moat незаметно вырождается в «наша команда» (FM.PS.003) |
| Знакомый Growth Model переоценивается | При выборе Growth Model (§2.3) внимание переоценивается тот канал, который уже знаком команде (например, founder из sales тяготеет к Sales-Led), и недооценивается объективное соответствие модели сегменту (ARPU, ACV) |

---

> 2026-07-23 — миграция на обогащённый формат карточки (Forces + Bias-Annotation), WP-448 Ф12. Эталон формата: `SPF/pack-template/03-methods/_method-card-template.md`.
