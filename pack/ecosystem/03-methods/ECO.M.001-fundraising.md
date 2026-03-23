---
id: ECO.M.001
title: Привлечение инвестиций (Fundraising)
type: method
status: active
created: 2026-03-21
updated: 2026-03-23
sota_status: enriched
s2r_families: [F7]
related:
  - "DS-ecosystem-development/A3.1.Meaning/3.1.1. Investment-Attraction/"
  - "WP-142"
  - "WP-145"
  - "ECO.D.001"
  - "ECO.SOTA.001"
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

## 7. YC First Minute Rule — Seed Pitch Construction

> Источник: YC Michael Seibel (Managing Director), 5000+ стартапов.

**Проблема:** 90% founders строят pitch по шаблону (Problem → Solution → Market → Team), но инвесторы решают в первую минуту.

**Метод:**

1. **Lead with Impressive** — первый слайд = самое сильное в компании:
   - Если есть traction → покажи growth graph с timeframe
   - Если есть team pedigree → покажи credentials
   - Если есть non-obvious insight → начни с него

2. **60-Second Clarity Test:**
   - Investor должен понять что ты делаешь за 60 сек
   - 2 предложения + 1 конкретный пример = impossible to misunderstand
   - Jargon = red flag (сигнал insecurity)

3. **Traction Must Have Timeframe:**
   - «Grew to 10K users» → ничего не значит
   - «Grew from 0 to 10K in 8 weeks» → impressive
   - Momentum = traction / time

4. **Design Principles:**
   - Legibility: читается с 5 метров
   - Simplicity: одна мысль на слайд
   - Obviousness: граф читается без объяснений
   - **Clarity 100% > Accuracy 100%:** лучше 80% accurate + 100% clear, чем наоборот

**Failure modes:**
- FM.FR.005: Template-following — по шаблону, теряя impressive-first
- FM.FR.006: Complexity flex — jargon → investor отключается
- FM.FR.007: Traction без timeframe — «10K users» без контекста

---

## 8. Bottom-Up SaaS Financial Projections

> Источник: Finro Financial, GoLimelight SaaS Forecasting Guide (2026)

**Проблема:** Top-down projections ($100B TAM × 1%) не работают с seed-инвесторами 2026. Хотят видеть unit economics.

**Формула:**
```
Revenue (month M) = Σ(Cohorts) × Conversion Rate × ARPU × Retention Curve
```

**Компоненты:**

1. **Cohort:** группа пользователей, acquired в одном месяце. Seed-stage: model 12-24 cohorts
2. **Conversion Rates:** Signup → Activation (40-60%) → Trial (20-40%) → Paid (10-25% EdTech 2026)
3. **ARPU:** $10-50/mo (B2C), $100-500/mo (B2B SMB). Model expansion: upsell 10-20%/year
4. **Retention Curve:** M1: 100%, M3: 60-70%, M12: 40-50%, M24: 30-40%

**2026 Benchmarks (Seed Stage <$1M ARR):**
- LTV: $500-2,000 (EdTech B2C)
- CAC payback: <12 months (отлично), <18 months (приемлемо)
- Burn multiple: <1.5x (отлично), <2x (хорошо), >3x (red flag)
- MoM growth: 15-25% (seed), 10-20% (Series A)

**Failure modes:**
- FM.FR.008: Top-down only — «$100B market × 1%» → мгновенный отказ
- FM.FR.009: Single-line forecast — «будем расти 10x/год» без cohort breakdown
- FM.FR.010: Vanity metrics — «10M users» без revenue per user
- FM.FR.011: No sensitivity analysis — единственный best-case сценарий

---

## 9. Investor Psychology (2026)

> Источник: YC, a16z, Sequoia 2026

**Топ приоритеты инвестора при первом просмотре:**
- **Traction > Deck:** ARR/users/engagement, не слайды
- **Bottom-up model:** реалистичные прогнозы (segment × conversion × ARPU)
- **Team credibility:** domain expertise или adjacent success
- **Problem-solution fit:** clear pain point, не «nice to have»

**Типичные причины отказа:**
- No traction ($0 ARR на seed = red flag 2026)
- Top-down financials
- Vague differentiation («AI-powered learning platform»)

---

## 10. Pitch Deck Structure (YC template 2026)

12 слайдов (10-15 мин):
1. **Problem:** созидатели тонут в complexity
2. **Solution:** IWE ecosystem (методология + платформа + сообщество)
3. **Why now:** AI agents = экзоскелет (усиливают мышление, не заменяют)
4. **Market:** EdTech $44.5B by 2026, niche = adult professional development
5. **Business model:** Red Hat (open methodology, paid infrastructure)
6. **Traction:** 13K users, $X ARR, Y% MoM growth
7. **Product:** Digital Twin + Agents + Руководства
8. **Competition:** Matrix (см. ECO.D.002)
9. **Go-to-market:** Community-led growth
10. **Financials:** Bottom-up ARR projection (3 years)
11. **Team:** Founders + advisors
12. **Ask:** $10M seed at $16M pre-money, 18-month runway

---

## 11. Term Sheet Essentials (Seed 2026)

- **Инструмент:** SAFE наиболее распространён. >$5M → priced equity (см. ECO.D.001)
- **Валюация:** $16M median pre-money (2026)
- **Discount:** 15-20% типично для SAFE
- **Pro-rata:** инвесторы хотят право на follow-on в Series A
- **Board:** нет мест на seed (observer rights ok)
- **Vesting:** 4 года с 1-year cliff (стандарт)
- **Liquidation preference:** 1x (не participating preferred)

---

## 12. TODO (для наращивания)

- [ ] Метод: due diligence checklist (что подготовить)
- [ ] Метод: investor outreach — pipeline и CRM
- [ ] Кейсы: успешные seed-раунды EdTech/Intelligence platforms 2024-2026
