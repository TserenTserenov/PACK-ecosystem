---
id: ECO.M.001
title: Привлечение инвестиций (Fundraising)
type: method
status: draft
created: 2026-03-21
updated: 2026-03-21
sota_status: initial
s2r_families: [F7]
related:
  - "DS-ecosystem-development/A3.1.Meaning/3.1.1. Investment-Attraction/"
  - "WP-142"
  - "WP-145"
---

# ECO.M.001: Привлечение инвестиций (Fundraising)

> **Назначение:** Source-of-truth для знаний о привлечении инвестиций в экосистему.
> **Статус:** initial — начальный сбор знаний. Будет расти итеративно.

---

## 1. Определение

Fundraising — метод привлечения внешнего капитала для масштабирования экосистемы. Включает: подготовку pitch materials, оценку компании, переговоры с инвесторами, structuring сделки.

**Различение:** Fundraising ≠ Продажи. Fundraising продаёт долю в будущем. Продажи продают продукт сейчас.

---

## 2. Ключевые термины (UL)

| Термин | Определение |
|--------|-------------|
| **Pitch deck** | Презентация (8-12 слайдов) для инвестора |
| **Elevator pitch** | Устное описание за ≤30 сек |
| **One-pager** | Одностраничное резюме для предварительного интереса |
| **Pre-money valuation** | Оценка компании ДО вложения инвестора |
| **Post-money valuation** | Pre-money + сумма инвестиций |
| **Dilution** | Размывание доли основателей при привлечении инвестиций |
| **Term sheet** | Документ с условиями сделки (до юридического оформления) |
| **SAFE** | Simple Agreement for Future Equity — упрощённый инструмент (YC) |
| **Convertible note** | Конвертируемый заём — долг, превращающийся в долю |
| **Cap table** | Таблица распределения долей между участниками |
| **Runway** | Время, на которое хватает денег (месяцы) |
| **Burn rate** | Ежемесячные расходы |
| **ARR** | Annual Recurring Revenue — годовая повторяющаяся выручка |
| **MRR** | Monthly Recurring Revenue — месячная |
| **LTV** | Lifetime Value — суммарная выручка от одного клиента |
| **CAC** | Customer Acquisition Cost — стоимость привлечения |
| **Traction** | Доказательства спроса (выручка, пользователи, рост) |
| **PMF** | Product-Market Fit — доказанное соответствие продукта рынку |
| **Series A/B/C** | Раунды финансирования по мере роста |

---

## 3. Раунды и стадии

| Стадия | Типичная сумма | Типичная оценка | Что доказывает |
|--------|---------------|-----------------|----------------|
| **Pre-seed** | $100K–$1M | $2-10M | Идея + команда + MVP |
| **Seed** | $1M–$10M | $5-50M | Traction + PMF signals |
| **Series A** | $10M–$30M | $30-100M | Proven PMF + repeatable growth |
| **Series B** | $30M–$100M | $100M+ | Scale + unit economics |

---

## 4. Структура pitch deck (SOTA)

**Sequoia framework (классика):**
1. Problem
2. Solution
3. Market (TAM/SAM/SOM)
4. Product
5. Traction
6. Team
7. Business model
8. Competition
9. Financials
10. Ask

**YC framework (минимализм):**
1. What do you do? (1 предложение)
2. How big is the market?
3. What's your progress?
4. What's unique about your approach?

---

## 5. Различения (fundraising-специфичные)

### D.FR.001: Traction ≠ Vanity metrics
- **Traction:** revenue, retention, NPS, paying customers, B2B contracts
- **Vanity:** downloads, registrations, page views, social followers

### D.FR.002: Valuation ≠ Revenue multiple
- На seed: оценка = потенциал × команда × moat, не просто N × ARR
- Фреймворк: Berkus, Scorecard, Risk Factor Summation

### D.FR.003: Dilution — не потеря, а обмен
- 20% за $10M при $50M post-money: основатели владеют 80% компании стоимостью $50M
- Правило: dilution 15-25% за раунд — нормально. >30% — красный флаг

### D.FR.004: PMF signals (seed stage)
- Retention >40% через 6 мес
- Organic growth (word-of-mouth)
- Платящие клиенты без скидок
- B2B-заказчики с повторными покупками
- NPS >50

---

## 6. Failure modes

| Ошибка | Последствие | Как избежать |
|--------|-------------|-------------|
| Завышенная оценка (pre-money) | Down round позже → потеря доверия | Benchmarks по стадии и отрасли |
| Нет clear ask (сумма + на что) | Инвестор не понимает что финансирует | Таблица: направление → сумма → результат |
| Traction gap (мало данных) | «Приходите когда подрастёте» | Показать trajectory, не snapshot |
| Слабая команда (нет бизнес-лидера) | «Кто будет продавать?» | Показать plan для найма или advisory |
| Нет competitor slide | «Наивные основатели» | Честная матрица: мы vs альтернативы |
| Прогнозы без обоснования | «Фантазии» | Bottom-up: сегмент × конверсия × ARPU |

---

## 7. TODO (для наращивания)

- [ ] Исследовать: типичные term sheet условия для seed EdTech
- [ ] Исследовать: успешные seed-раунды EdTech/Intelligence platforms 2024-2026
- [ ] Исследовать: investor psychology — что смотрят первым в deck
- [ ] Различение: SAFE vs convertible note — когда что
- [ ] Метод: due diligence checklist (что подготовить)
- [ ] Метод: investor outreach — pipeline и CRM
- [ ] Паттерн: bottom-up financial projections
