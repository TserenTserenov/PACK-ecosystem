---
id: ECO.M.002
name: "Canvas Selection Method"
type: method
status: active
created: 2026-03-23
last_updated: 2026-07-23
source: "Miro, Creately, Ash Maurya, Scout 22 мар 2026"
related: [ECO.D.002]
s2r_families: [F4, F7]
---

# ECO.M.002: Canvas Selection Method

## Forces

_(Optional, WP-448 Ф12) Какие конкурирующие давления удерживает метод._

| Force | Tension |
|-------|---------|
| Скорость итерации (Lean Canvas, 20 мин, weekly) ↔ строгость стратегического планирования (BMC, 1-2ч, quarterly) | Decision Tree разводит выбор по стадии (pre-PMF vs post-PMF), но сама скорость Lean Canvas делает его непригодным там, где нужен BMC-уровень детализации |
| Внутренняя валидация гипотез ↔ внешняя легитимность | Lean Canvas с red/yellow/green — инструмент команды; BMC явно указан как то, что нужно «Share with stakeholders/investors» — один и тот же артефакт не решает обе задачи одновременно |
| Один канвас на всё время ↔ переход между канвасами | «Best Practice 2026: Use both sequentially» — переход от Lean Canvas к BMC после PMF рискует потерей нюансов провалидированных допущений (Transfer validated insights), если миграция не формализована |

## Decision Tree

```
Are you pre-product-market fit?
  ├─ YES → Lean Canvas
  │   ├─ Fill in 20 min
  │   ├─ Identify riskiest assumption (Problem? Solution? Channel?)
  │   ├─ Test assumption (MVP, interview, landing page)
  │   └─ Iterate weekly
  │
  └─ NO → Business Model Canvas
      ├─ Fill in 1-2 hours with team
      ├─ Use for strategic planning
      ├─ Share with stakeholders/investors
      └─ Update quarterly
```

## Best Practice 2026: Use both sequentially

1. **Months 0-18:** Lean Canvas для validation
   - Weekly updates
   - Focus: Problem-Solution Fit → Product-Market Fit
   - Red/Yellow/Green для каждого блока (validated / hypothesis / unknown)

2. **After PMF:** Transfer validated insights в BMC
   - BMC становится strategic planning tool
   - Quarterly updates
   - Share with investors, team, partners

## Применение к IWE (2026)

- **Сейчас:** Lean Canvas (ещё validating unit economics, channel strategy, retention model)
- **После seed round:** BMC (структурировать для команды, investors)

## Источники

- [Miro: Lean Canvas vs BMC](https://miro.com/strategic-planning/lean-canvas-vs-business-model-canvas/)
- [Creately: When to Use Each Canvas](https://creately.com/guides/lean-canvas-vs-business-model-canvas/)

## Bias-Annotation

_(Optional, WP-448 Ф12) Куда систематически съезжает внимание практикующего._

| Bias | Direction of distortion |
|------|--------------------------|
| Полнота заполнения вместо риска | Внимание съезжает на аккуратное заполнение всех блоков Lean Canvas вместо фокуса на «riskiest assumption» (Problem/Solution/Channel), которую Decision Tree требует тестировать в первую очередь |
| Соблазн выглядеть «серьёзно» | Привлекательность BMC как более солидного артефакта смещает практика к преждевременному переходу на BMC ещё до PMF (см. «После seed round: BMC» в «Применение к IWE») — статус канваса подменяет реальный статус валидации |

---

> 2026-07-23 — миграция на обогащённый формат карточки (Forces + Bias-Annotation), WP-448 Ф12. Эталон формата: `SPF/pack-template/03-methods/_method-card-template.md`.
