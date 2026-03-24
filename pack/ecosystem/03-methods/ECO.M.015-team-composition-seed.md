---
id: ECO.M.015
title: "Team Composition for Seed-Stage Startup"
type: method
status: active
created: 2026-03-24
source: "Andrew Chen Seed Team, Dover First 5 Hires 2026, Dover Seed Hiring 2025, DBB MVP Team Guide, Octopus Ventures Pre-Seed Teams, Dover Hiring Trends 2026"
related: [ECO.M.016, ECO.SOTA.007]
s2r_families: [F9]
---

# ECO.M.015: Team Composition for Seed-Stage Startup

> **Назначение:** Метод определения оптимального состава команды на seed-стадии — кого нанимать, в каком порядке и с каким профилем.

---

## 1. Принцип

На seed-стадии каждый новый член команды = ~20% компании. Найм определяет скорость, культуру и направление. Ошибка в найме на seed = экзистенциальный риск.

**Принцип 2025-2026:** Runway precious → каждый hire critical. Think 12-18 months ahead, hire people who can grow into future roles.

---

## 2. Первые 5 найм

> Порядок зависит от того, что уже есть у основателей.

### Приоритет 1: Закрыть core gap

| Если основатель... | Первый найм |
|------|-------------|
| Technical (может кодить full-time) | Первый нон-technical hire (marketing или sales) |
| Non-technical | **Engineer #1** (самый критичный hire) |
| Solo | **Co-founder** или senior generalist |

### Приоритет 2-5: Build core team

| # | Роль | Профиль | Зачем |
|---|------|---------|-------|
| 2 | **Engineer #2** | Full-stack, shipping-oriented | Параллельная разработка, code review |
| 3 | **Growth / Marketing** | Content + analytics, T-shaped | Inbound pipeline, SEO, community |
| 4 | **Product / Design** | UX researcher + designer | User interviews, prototype, design system |
| 5 | **Ops / CS** | Generalist, process-oriented | Customer success, operations, glue work |

### Sales vs Marketing: decision rule

- **ACV >$50K** (enterprise, multi-demo sales cycle) → **Salesperson** first
- **ACV <$10K** (self-serve, credit card signup) → **Marketing** first

---

## 3. Hiring Profile на Seed

### Что искать

| Качество | Почему критично |
|----------|----------------|
| **Execution-oriented** | Нет места для «философов» — нужен immediate impact |
| **Comfortable with ambiguity** | Нет процессов, нет roadmap — нужно фигурить |
| **T-shaped** | Глубина в 1 области + breadth для cover других |
| **Mission-aligned** | Стартап = трудно и долго → мотивация = залог retention |
| **Growth potential** | Team lead / Director level — достаточно senior для ownership, достаточно junior для hands-on |

### Что НЕ искать

| Антипаттерн | Почему опасно |
|-------------|---------------|
| VP/C-level из корпорации | Привык к ресурсам и процессам, которых нет |
| «Idea person» без execution | Идеи не дефицит — execution дефицит |
| Specialist-only | На seed нужны generalists |
| Culture fit-only (без skill) | Хорошие люди без навыков → медленно |

---

## 4. Модели найма

| Модель | Когда | Стоимость | Risk |
|--------|-------|-----------|------|
| **Full-time** | Core roles (eng, product) | Высокая (salary + equity) | Низкий (commitment) |
| **Fractional** | Специализированные (recruiter, CFO, legal) | Средняя (hourly) | Средний |
| **Contract** | Temporary burst (design sprint, content) | Средняя | Средний (no ownership) |
| **AI-augmented** | Repetitive tasks (code gen, content, analytics) | Низкая | Низкий (не замена, а leverage) |

### SOTA 2026: AI как «team member»

AI tools (Claude Code, Cursor, Copilot) → 1 engineer = output of 2-3. Это значит:
- Можно дольше оставаться lean (2-3 инженера вместо 5-7)
- Первые нон-engineering hires можно делать раньше
- Fractional + AI > full-time mediocre hire

---

## 5. Org Structure на Seed

```
Founder(s)
├── Engineering (2-3)
├── Growth/Marketing (1)
├── Product/Design (1, часто founder)
└── Ops/CS (1, часто founder)
```

**Нет:** Менеджеров, HR, отдельного QA, DevOps (всё на инженерах + CI/CD + AI).
**Решения:** Founder делает всё, что не делегировано. Decision-making = founder-led.

---

## 6. Применение к IWE

| Роль | Текущее | Потребность |
|------|---------|------------|
| Founder/Strategist | Tseren | ✅ |
| Engineering | AI-augmented (Claude Code) | ⚠️ Engineer #1 при масштабировании |
| Community/Ops | Клуб, бот | ⚠️ Community manager при росте |
| Content/Growth | Founder-led | ⚠️ Content/growth hire при GTM |
| Product/UX | Founder-led | Позже (Series A) |

---

## 7. Failure modes

| ID | Ошибка | Последствие |
|----|--------|-------------|
| FM.TC.001 | Hire too many too fast | Burn rate ↑, coordination cost ↑, culture dilution |
| FM.TC.002 | Hire too senior (VP from BigCo) | Ожидания ≠ реальность, quick departure |
| FM.TC.003 | Hire only friends | Skill gaps, groupthink, hard conversations avoided |
| FM.TC.004 | No equity for early hires | No skin in game → mercenary culture |
| FM.TC.005 | Hire before PMF | Scaling what doesn't work |
| FM.TC.006 | Ignore AI leverage | 2× headcount where 1× + AI sufficient |
