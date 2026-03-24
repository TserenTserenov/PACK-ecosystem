---
id: ECO.M.013
title: "Feedback Loops (User → Product → Ecosystem)"
type: method
status: active
created: 2026-03-24
source: "Teresa Torres Continuous Discovery, ProductTalk 2026 Roadmap, Stack Overflow Continuous Discovery, IxDF Continuous Discovery, Pendo Product Discovery 2025"
related: [ECO.M.012, ECO.M.010]
s2r_families: [F6]
---

# ECO.M.013: Feedback Loops (User → Product → Ecosystem)

> **Назначение:** Метод построения циклов обратной связи, обеспечивающих непрерывное улучшение экосистемы на основе реальных данных от участников.

---

## 1. Определение

Feedback loop — замкнутый цикл: сбор данных → анализ → решение → изменение → наблюдение результата → повторный сбор. В экосистеме feedback loops работают на трёх уровнях: пользователь → продукт, продукт → экосистема, экосистема → стратегия.

**Различение:** Feedback ≠ Data collection. Data collection — сбор. Feedback loop — замкнутый цикл, где данные приводят к изменениям, а результат изменений снова измеряется.

---

## 2. Три уровня feedback loops

| Уровень | Цикл | Скорость | Кто действует |
|---------|------|----------|---------------|
| **L1: User → Product** | Пользователь даёт feedback → продукт меняется | Дни-недели | Product team |
| **L2: Product → Ecosystem** | Продуктовые метрики → изменение экосистемы (новые компоненты, партнёры) | Недели-месяцы | Ecosystem team |
| **L3: Ecosystem → Strategy** | Здоровье экосистемы → стратегические решения (pivot, expand, prune) | Месяцы-кварталы | Leadership |

---

## 3. L1: User → Product (Continuous Discovery)

### Метод Teresa Torres (SOTA 2025-2026)

> Discovery и Delivery работают параллельно, а не последовательно.

**Еженедельный ритм:**
1. **Интервью** — минимум 1 user interview в неделю (не «раз в квартал»)
2. **Opportunity mapping** — визуализация пользовательских нужд (Opportunity Solution Tree)
3. **Assumption testing** — проверка рискованных предположений до разработки
4. **Prototype testing** — быстрая валидация решений

### Каналы сбора (IWE)

| Канал | Тип feedback | Скорость |
|-------|-------------|----------|
| Bot inline feedback (👍/👎) | Количественный, immediate | Секунды |
| Discourse posts/topics | Qualitative, organic | Часы |
| NPS survey (quarterly) | Количественный, structured | Квартал |
| User interview | Qualitative, deep | Неделя |
| Support tickets | Qualitative, problem-driven | Дни |
| Analytics (behavior) | Quantitative, passive | Continuous |

### Closing the loop

> Пользователи, которые видят свой feedback реализованным, становятся лояльными.

- **Announce changes:** «Вы просили → мы сделали» (changelog, клуб)
- **Tag requesters:** Уведомить конкретных пользователей, чей feedback реализован
- **Measure impact:** Метрика до/после изменения

---

## 4. L2: Product → Ecosystem

| Сигнал | Реакция экосистемы |
|--------|-------------------|
| Высокий churn на этапе X | Добавить компонент (mentor, AI coach) на этом этапе |
| Пользователи просят функцию вне scope | Партнёрство или marketplace opportunity |
| Retention высокий в community, низкий в product | Усилить связь product ↔ community |
| API usage растёт | Инвестировать в DX (ECO.M.009) |

---

## 5. L3: Ecosystem → Strategy

| Сигнал | Стратегическое решение |
|--------|----------------------|
| Ecosystem Health Score <30 | Кризисный пересмотр ценности |
| Contribution растёт | Инвестировать в creator tools |
| Net growth отрицательный 2+ мес | Ревью positioning и value proposition |
| Partner demand растёт | Формализовать partner program |
| Один компонент доминирует | Риск хрупкости — диверсифицировать |

---

## 6. Feedback Infrastructure

### Minimal Viable Feedback System

| Компонент | Инструмент | Стоимость |
|-----------|-----------|-----------|
| Quantitative (NPS, CSAT) | Bot survey + Neon DB | Бесплатно |
| Qualitative (organic) | Discourse topics tagged [feedback] | Бесплатно |
| Behavioral | Analytics (Grafana + custom events) | Бесплатно |
| Deep (interviews) | Calendly + Zoom | ~$15/мес |
| Aggregation | Weekly review (manual → AI-assisted) | Time |

### AI-Assisted Feedback Processing (SOTA 2026)

- Auto-categorize feedback topics (LLM classification)
- Sentiment analysis on community posts
- Auto-summarize weekly feedback themes
- Suggest opportunity areas based on patterns

---

## 7. Антипаттерны

| Антипаттерн | Проблема | Решение |
|-------------|---------|---------|
| **Feedback graveyard** | Собираем, но не анализируем | Weekly review ritual |
| **Loudest voice wins** | Строим для vocal minority | Weight by segment size + frequency |
| **Survey fatigue** | Слишком часто спрашиваем | Max 1 structured survey / quarter |
| **One-way communication** | Собираем, но не показываем результат | «Вы просили → мы сделали» |
| **Confirmation bias** | Ищем feedback, подтверждающий наше решение | Actively seek disconfirming evidence |

---

## 8. Failure modes

| ID | Ошибка | Последствие |
|----|--------|-------------|
| FM.FL.001 | Нет регулярного ритма сбора | Feedback случайный, не систематический |
| FM.FL.002 | Discovery после Delivery | Строим → спрашиваем → поздно менять |
| FM.FL.003 | Только quantitative | Знаем «что», не знаем «почему» |
| FM.FL.004 | Только qualitative | Знаем «почему» от 5 человек, не знаем масштаб |
| FM.FL.005 | Feedback loop не замкнут | Пользователь не видит результат → перестаёт давать feedback |
