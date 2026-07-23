---
id: ECO.M.008
title: "Build vs Buy vs Partner Decision Framework"
type: method
status: active
created: 2026-03-24
last_updated: 2026-07-23
source: "TheCodev Build vs Buy Framework, Engenia Tech 2026, Pragmatic Institute, AppInventiv 2026, Sedulo Group F1 Framework, DevPro Journal ISV 2026"
related: [ECO.M.007, ECO.M.009]
s2r_families: [F8]
---

# ECO.M.008: Build vs Buy vs Partner Decision Framework

> **Назначение:** Метод принятия решения при появлении новой capability — строить самим, покупать готовое или входить в партнёрство.

---

## 1. Определение

Build vs Buy vs Partner — стратегическая модель оценки трёх путей получения новой возможности (capability) для экосистемы. Традиционный «Build vs Buy» расширен третьей опцией — Partner — особенно актуальной в эпоху SaaS и API-экономики.

**Принцип 2026:** «Do fewer things in-house but do them exceptionally well. Be the best in the world at 3-5 core capabilities and buy or partner for everything else.»

---

## Forces

_(Optional, WP-448 Ф12) Какие конкурирующие давления удерживает метод._

| Force | Tension |
|-------|---------|
| Скорость получения capability ↔ долгосрочная стоимость владения | Buy/Partner быстрее (§2 Time-to-market), но «Стоимость (долгосрочная)» растёт (subscription, vendor lock-in), тогда как Build дороже сейчас, но дешевле при владении (§2) |
| Контроль/дифференциация ↔ дисциплина «меньше, но отлично» | Желание строить всё самому (Control, §3 Decision Matrix) конкурирует с принципом 2026 «3-5 core capabilities» (§1) — соблазн build за пределами core ведёт к FM.BBP.001 |
| Видимая цена лицензии ↔ скрытая стоимость интеграции | Buy кажется дешёвым по subscription, но Hidden Iceberg Framework (§6) показывает integration/migration/training/compliance costs, не видные при выборе |

---

## 2. Три пути

| | Build | Buy | Partner |
|---|---|---|---|
| **Что** | Разработка in-house | Приобретение готового решения (SaaS, лицензия, M&A) | Интеграция через API/партнёрство |
| **Контроль** | Полный | Зависит от вендора | Разделённый |
| **Time-to-market** | Медленный (недели-месяцы) | Быстрый (дни-недели) | Средний (зависит от API quality) |
| **Стоимость (краткосрочная)** | Высокая (dev team time) | Средняя (subscription) | Низкая (integration effort) |
| **Стоимость (долгосрочная)** | Низкая (владение) | Растущая (vendor lock-in) | Средняя (зависимость от партнёра) |
| **Когда** | Core differentiator | Proven capability, нужна скорость | Access to market/technology |

---

## 3. Decision Matrix (5 критериев)

Оценить каждый вариант по шкале 1-5:

| Критерий | Build | Buy | Partner |
|----------|-------|-----|---------|
| **Control** (владение, кастомизация) | ? | ? | ? |
| **Cost** (TCO за 3 года) | ? | ? | ? |
| **Speed** (time-to-value) | ? | ? | ? |
| **Scalability** (масштабирование) | ? | ? | ? |
| **Risk** (обратный: чем меньше риск, тем выше балл) | ? | ? | ? |

**Правило:** Не выбирать самый быстрый вариант — выбирать тот, что даёт **sustainable value**.

### Взвешивание по стадии

| Стадия | Приоритетные критерии |
|--------|----------------------|
| Pre-seed / Seed | Speed, Cost |
| Series A | Scalability, Control |
| Growth | Control, Risk |

---

## 4. Правила выбора

### Build когда:

- Capability — **core differentiator** (то, что отличает от конкурентов)
- Решение не существует на рынке или не подходит
- Нужен полный контроль над данными и UX
- Есть компетенция в команде

### Buy когда:

- Capability — **commodity** (аутентификация, платежи, email)
- Time-to-market критичен
- Рынок предлагает proven solutions
- Стоимость Build > стоимость Buy за 3 года

### Partner когда:

- Нужен доступ к рынку или технологии, которой нет
- Capability усиливается совместно (win-win)
- API/интеграция достаточна (не нужен full ownership)
- Стратегические отношения важнее тактического решения

---

## 5. Применение к IWE

| Capability | Решение | Обоснование |
|-----------|---------|-------------|
| **Методология** | Build | Core differentiator, нет аналогов |
| **LMS (Aisystant)** | Build | Core differentiator, специфичный UX |
| **Identity (Ory)** | Buy (open-source) | Commodity, proven solution |
| **AI/LLM** | Partner (Anthropic, OpenAI) | API-интеграция, не нужен own model |
| **Платежи** | Buy (Stripe/Tinkoff) | Commodity, регуляторные требования |
| **Community** | Build + Partner | Discourse (Buy) + своя модерация (Build) |
| **Аналитика** | Buy (Grafana) + Build (Digital Twin) | DT = differentiator, Grafana = commodity |
| **CI/CD** | Buy (Railway, GitHub Actions) | Commodity, focus on product |

---

## 6. Hidden Iceberg Framework (DevPro 2026)

> «Видимые 10% — стоимость лицензии. Невидимые 90% — интеграция, обучение, миграция, поддержка.»

При оценке Buy учитывать:
- **Integration cost:** Время на подключение к существующему стеку
- **Migration cost:** Стоимость перехода при смене вендора
- **Training cost:** Обучение команды
- **Compliance cost:** Соответствие требованиям (GDPR, data residency)
- **Opportunity cost:** Что могли бы сделать вместо интеграции

---

## 7. Периодический пересмотр

Решение Build/Buy/Partner — не финальное. Пересматривать при:
- Смене стадии (seed → Series A)
- Появлении нового решения на рынке
- Изменении core capabilities
- Vendor risk (sunset, pricing change, acquisition)

**Антипаттерн:** «Мы уже это построили, значит продолжаем поддерживать» (sunk cost). Если commodity-решение стало лучше вашего — мигрируйте.

---

## Bias-Annotation

_(Optional, WP-448 Ф12) Куда систематически съезжает внимание практикующего. Не дублирует `## 8. Failure modes` — там «что пойдёт не так», здесь «куда дрейфует внимание»._

| Bias | Direction of distortion |
|------|--------------------------|
| Видимая цена важнее скрытых издержек | Внимание смещается к цене лицензии/subscription (§2 таблица) и недооценивается Hidden Iceberg costs (§6: интеграция, миграция, обучение, compliance) — считается то, что в счёте, а не то, что съедает бюджет позже |
| Control-критерий переоценивается при Build | «Мы не хотим зависеть от вендора» звучит убедительно и смещает баланс Decision Matrix (§3) в пользу Build, даже когда взвешенная оценка Cost/Speed/Scalability/Risk указывает на Buy/Partner |
Пересмотр решения дороже политически, чем технически | Отказаться от Build/Partner значит признать перед стейкхолдерами, что бюджет и headcount на решение (§3) были потрачены на то, что теперь меняют, — внимание уходит от триггеров пересмотра (§7) не потому что решение «кажется постоянным», а потому что поднимать вопрос социально дороже, чем не поднимать |

---

## 8. Failure modes

| ID | Ошибка | Последствие |
|----|--------|-------------|
| FM.BBP.001 | Build всё (NIH-синдром) | Медленно, дорого, отвлекает от core |
| FM.BBP.002 | Buy core differentiator | Потеря конкурентного преимущества, vendor lock-in на ядре |
| FM.BBP.003 | Не учитывать Hidden Iceberg | Бюджет x3-5 от ожидаемого |
| FM.BBP.004 | Partner без exit strategy | Зависимость без возможности миграции |
| FM.BBP.005 | Не пересматривать решения | Legacy tools тормозят команду |

---

> 2026-07-23 — миграция на обогащённый формат карточки (Forces + Bias-Annotation), WP-448 Ф12. Эталон формата: `SPF/pack-template/03-methods/_method-card-template.md`.
