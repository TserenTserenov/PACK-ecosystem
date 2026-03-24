---
id: ECO.M.001
title: Привлечение инвестиций (Fundraising)
type: method
status: active
created: 2026-03-21
updated: 2026-03-24
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
- Founder secondary на ранних стадиях без доказанного traction (отвлекает от транша, воспринимается как red flag)

**Правила инвестиционного нарратива (vs публицистика/vision):**
- Инвестор хочет: один продукт → одна цена → одна динамика роста → на что пойдёт транш в первые 6 мес
- Vision = допустим, но цифры должны быть конкретными: «$10/мес сейчас, 500 платящих, $60K ARR» — не «больше-меньше»
- Founder secondary обсуждается после доказанного успеха вложения, не в первом deck

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

## 12. Due Diligence — что подготовить (Seed 2025–2026)

> Источники: 4Degrees, Kruze Consulting, Papermark, StartUpNV, Zyner.io

**Принцип:** Инвестор проверяет 6 областей. На seed — облегчённая версия, но data room обязателен.

### 6 областей проверки

| Область | Что проверяют | Seed-minimum |
|---------|--------------|--------------|
| **1. Финансы** | P&L, cash flow, burn rate, runway, unit economics | Финмодель (bottom-up) + актуальный P&L + cap table |
| **2. Продукт и рынок** | PMF signals, retention, TAM/SAM, competitive positioning | Метрики (retention, NPS, MoM growth) + competitive matrix |
| **3. Команда** | Founder-market fit, domain expertise, org structure | Био основателей + advisory board + hiring plan |
| **4. Юридическое** | Incorporation, IP ownership, contracts, litigation | Свидетельство о регистрации + IP assignment + SAFE/notes |
| **5. Технология** | Architecture, scalability, security, tech debt | Архитектурная схема + security baseline |
| **6. Операции** | Processes, key risks, insurance | PROCESSES.md + risk register (минимальный) |

### Data Room — структура папок

```
00_Intro/          — pitch deck, one-pager, executive summary
01_Corporate/      — incorporation docs, cap table, bylaws
02_Financials/     — P&L, cash flow, financial model, use of funds
03_Legal/          — SAFE/notes, IP assignments, key contracts
04_Product/        — architecture, roadmap, metrics dashboard
05_Team/           — bios, org chart, hiring plan, vesting schedules
06_Customers/      — testimonials, case studies, NPS data
07_Compliance/     — privacy policy, ToS, licenses
```

**Инструменты:** Notion, Google Drive, Papermark (аналитика просмотров). На seed достаточно Google Drive с чёткой структурой.

### Failure modes (due diligence)

| Ошибка | Последствие |
|--------|-------------|
| FM.FR.012: Нет data room до первой встречи | Инвестор просит — задержка 2-3 недели → потеря momentum |
| FM.FR.013: Cap table с ошибками | Red flag → углублённая юридическая проверка → отказ |
| FM.FR.014: IP не оформлен на компанию | Стоп-фактор. Инвестор не закроет сделку без IP assignment |

---

## 13. Investor Outreach — Pipeline и CRM

> Источники: Visible.vc, TechStars, Prospeo, Future Ventures, HubSpot/LinkedIn Benchmark

### Воронка инвестора

```
Target list (100-200)
  → Outreach / Intro (warm preferred)
    → First meeting (10-15%)
      → Follow-up / Materials shared (50-60% от встреч)
        → Due diligence (20-30% от follow-up)
          → Term sheet (30-50% от DD)
            → Close (80-90% от term sheet)
```

**Ключевой бенчмарк:** 5-10% конверсия от target list до close. На 1 закрытого инвестора нужно 10-20 первых встреч и 100+ контактов в pipeline.

### Стадии pipeline (CRM)

| Стадия | Действие | Типичное время |
|--------|----------|---------------|
| **1. Research** | Составить long list (100-200), отфильтровать по: стадия, сектор, чек, география | 1-2 недели |
| **2. Warm intro** | Через общих знакомых, портфельные компании, LinkedIn | Приоритет #1 — конверсия 3-5x выше cold |
| **3. Cold outreach** | Персонализированное письмо: 3 предложения (что делаем, traction, ask) | Конверсия в ответ: 5-10% |
| **4. First meeting** | 30 мин. Цель: не закрыть сделку, а получить second meeting | — |
| **5. Follow-up** | Материалы (deck, one-pager, metrics) в течение 24ч | — |
| **6. Deep dive** | 60 мин. Product demo, финмодель, team deep dive | — |
| **7. Due diligence** | Data room открыт, вопросы, reference calls | 2-6 недель |
| **8. Term sheet** | Переговоры по условиям | 1-2 недели |
| **9. Close** | Юридическое оформление | 2-4 недели |

### CRM для seed-стартапа

| Инструмент | Для кого | Цена |
|------------|---------|------|
| Google Sheets / Notion | Pre-seed, <50 контактов | Бесплатно |
| OpenVC CRM | Seed, fundraising-focused | Бесплатно |
| Visible.vc | Seed+, investor updates + pipeline | $50+/мес |
| HubSpot Startup | Scale, полный CRM | Бесплатно (для стартапов) |

### Failure modes (outreach)

| Ошибка | Последствие |
|--------|-------------|
| FM.FR.015: Массовая рассылка без персонализации | Spam-репутация, 0% конверсия |
| FM.FR.016: Нет warm intro strategy | Cold-only → 3-5x ниже конверсия |
| FM.FR.017: Pipeline <50 контактов | Математически недостаточно для закрытия раунда |
| FM.FR.018: Нет follow-up в 24ч | Investor interest decays exponentially |

---

## 14. Кейсы: EdTech seed-раунды 2024–2026

> Источники: Reach Capital, DreamXWeb, TechCrunch, Crunchbase

### Benchmark: средний seed в EdTech

| Показатель | 2024 | 2025–2026 |
|-----------|------|-----------|
| Средний seed (non-AI) | ~$4M | ~$4-5M |
| Средний seed (AI-native) | ~$7.8M | ~$8-10M |
| Post-money valuation | $16-20M | $20-30M (AI-native) |

### Кейсы

**Speak** (AI language learning)
- OpenAI-backed, $1B valuation (дек 2024)
- 10M+ registered users, 1B+ sentences spoken в AI
- 95% accuracy в error detection
- Урок: voice-first AI + measurable outcomes = premium valuation

**MagicSchool AI** (K-12 AI tools)
- $45M raised (2025), начиналась как Replit-прототип
- Fastest-growing EdTech in K-12
- Урок: быстрый MVP → teacher adoption → funding follows traction

**Jotit** (handwriting + digital learning)
- $10M seed (Owl Ventures lead, 2025)
- Нишевый продукт: handwriting recognition + learning
- Урок: нишевой фокус + strong lead investor = successful seed

**Duolingo** (benchmark, public)
- $1B+ ARR (2025), 50M DAU, 11.5M paid subscribers
- 148 новых AI-powered курсов (апр 2025)
- Урок: gamification + AI + massive free tier → 2% conversion = profitable

### Паттерны успешных seed-раундов EdTech 2024–2026

1. **AI-native > AI-enhanced:** Продукты, построенные вокруг AI (не AI как фича), получают 2x оценку
2. **Measurable outcomes:** Retention, learning gains, time-to-competency — не vanity metrics
3. **Teacher/learner adoption first:** Traction через word-of-mouth, не paid marketing
4. **Niche → expand:** Узкий фокус на старте → расширение после PMF

---

## 15. TODO (для наращивания)

- [ ] Метод: negotiation tactics (term sheet переговоры)
- [ ] Метод: investor update template (monthly/quarterly)
- [ ] SOTA: свежие данные по EdTech funding Q1 2026
