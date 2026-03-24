---
id: ECO.M.018
title: "Platform Design Toolkit (Boundaryless)"
type: method
status: active
created: 2026-03-24
source: "Simone Cicero / Boundaryless PDT Framework, Boundaryless Ecosystem Canvas, Boundaryless Flywheel Sketching, McKinsey Ecosystem Strategy, Wardley Maps"
related: [ECO.M.007, ECO.M.002, ECO.D.005, ECO.M.006]
s2r_families: [F4, F5]
---

# ECO.M.018: Platform Design Toolkit (Boundaryless)

> **Назначение:** Набор canvas-инструментов для проектирования экосистемной стратегии — от идентификации участников до flywheel и control points. Специфичен для платформ и экосистем (не для одиночного продукта).

---

## 1. Определение

Platform Design Toolkit (PDT) — методология и набор canvas'ов для проектирования платформенных и экосистемных стратегий. Разработан Simone Cicero и командой Boundaryless.

**Различение:** PDT ≠ Lean Canvas / BMC. Lean Canvas и BMC проектируют бизнес-модель *одного продукта*. PDT проектирует *систему взаимодействий* между несколькими типами участников.

**Источник:** [boundaryless.io/pdt-framework](https://www.boundaryless.io/pdt-framework/)

---

## 2. Компоненты PDT

### 2.1 Ecosystem Canvas

Картирование всех участников экосистемы и их ценностных обменов.

| Элемент | Вопрос | Пример (IWE) |
|---------|--------|---------------|
| **Peer Consumers** | Кто потребляет ценность? | Студенты, практики |
| **Peer Producers** | Кто создаёт ценность? | Менторы, авторы контента |
| **Partners** | Кто усиливает платформу? | LMS, AI providers |
| **Value Exchanges** | Что обменивают участники? | Знания ↔ деньги, контент ↔ репутация |
| **Channels** | Через что происходит обмен? | Bot, LMS, Club |

### 2.2 Platform Strategy Model Canvas

Стратегический уровень: как платформа создаёт и захватывает ценность.

| Блок | Содержание |
|------|-----------|
| **Arena** | JTBD на уровне экосистемы (не одного продукта) |
| **Entities** | Типы участников (до 5) |
| **Value Propositions** | Отдельный VP для каждого типа участника |
| **Interactions** | Ключевые взаимодействия между участниками |
| **Channels & Context** | Как и где происходят взаимодействия |
| **Governance** | Правила, trust, quality control |
| **Key Metrics** | North Star + metrics по каждой стороне |

### 2.3 Flywheel Sketching Canvas

Визуализация самоусиливающегося цикла роста.

```
Больше студентов → Больше данных для Digital Twin →
  → Лучше персонализация → Лучше outcomes →
    → Больше word-of-mouth → Больше студентов → ...
```

**Правило:** Flywheel должен содержать cross-side network effect (ценность для одной стороны создаётся другой стороной).

### 2.4 Wardley Maps (интегрированный слой)

Картирование value chain от пользовательской потребности до компонентов, с учётом зрелости каждого компонента (genesis → custom → product → commodity).

**Применение в PDT:** Определение control points — компонентов, владение которыми даёт стратегическое преимущество.

---

## 3. Процесс PDT (5 шагов)

| Шаг | Действие | Canvas |
|-----|---------|--------|
| 1 | **Arena Definition** | Определить JTBD на уровне экосистемы |
| 2 | **Ecosystem Mapping** | Ecosystem Canvas: участники, обмены |
| 3 | **Strategy Design** | Platform Strategy Model: VP по сторонам, governance |
| 4 | **Flywheel Design** | Flywheel Sketching: self-reinforcing loop |
| 5 | **Control Point Analysis** | Wardley Map: где наше стратегическое преимущество |

---

## 4. PDT vs другие canvas-инструменты

| | Lean Canvas | BMC | PDT |
|---|---|---|---|
| **Scope** | 1 продукт | 1 бизнес | Экосистема (N участников) |
| **Стороны** | 1 (клиент) | 1 (клиент + партнёры) | 3-5 типов участников |
| **Network effects** | Нет | Нет | Встроены (cross-side, same-side) |
| **Flywheel** | Нет | Нет | Да |
| **Control points** | Нет | Нет | Да (Wardley Maps) |
| **Когда** | Pre-PMF, single product | Бизнес-модель | Platform/ecosystem стратегия |

---

## 5. Применение к IWE

### Ecosystem Canvas (IWE)

| Роль | Кто | Value получает | Value создаёт |
|------|-----|---------------|---------------|
| **Consumer** | Студенты, практики | Знания, навыки, сертификация, сообщество | Данные, feedback, плата |
| **Producer** | Менторы, авторы | Доход, репутация, teaching practice | Контент, менторство, экспертиза |
| **Partner (tech)** | AI providers, LMS | Distribution, data | Инфраструктура, AI capabilities |
| **Partner (content)** | Университеты, эксперты | Платформа распространения | Курсы, методологии |
| **Platform** | IWE team | — | Orchestration, бесшовность, governance |

### Control Points (Wardley)

| Компонент | Зрелость | Control? |
|-----------|----------|----------|
| Методология сист. мышления | Genesis/Custom | ✅ **Core differentiator** |
| Digital Twin | Custom | ✅ **Proprietary data moat** |
| LMS (Aisystant) | Custom/Product | ⚠️ Частичный |
| AI/LLM | Product/Commodity | ❌ Buy/Partner |
| Community (Discourse) | Commodity | ❌ Buy |
| Identity (Ory) | Commodity | ❌ Buy |

---

## 6. Связь с McKinsey Ecosystem Strategy

McKinsey дополняет PDT на стратегическом уровне:
- **Горизонтальное картирование:** все участники экосистемы в одной value chain
- **Вертикальное картирование:** глубина интеграции с каждым участником
- **Control points:** не просто «что у нас уникальное», а «какие позиции в value chain мы можем контролировать»
- **Governance:** Onboarding → Certification → Tiered compliance для партнёров

---

## 7. Failure modes

| ID | Ошибка | Последствие |
|----|--------|-------------|
| FM.PDT.001 | Использовать Lean Canvas для экосистемы | Не видим multi-sided dynamics, network effects |
| FM.PDT.002 | Ecosystem Canvas без flywheel | Статичная карта, нет self-reinforcing growth |
| FM.PDT.003 | Flywheel без control points | Рост без защиты — конкуренты копируют |
| FM.PDT.004 | Canvas как разовое упражнение | Экосистема меняется — canvas нужно обновлять |
| FM.PDT.005 | Слишком много типов участников (>5) | Complexity → невозможно управлять |
