---
id: ECO.M.005
title: "Оценка рынка: TAM / SAM / SOM"
type: method
status: active
created: 2026-03-24
source: "Antler, SeedBlink, GoingVC, Qubit Capital, ICanPitch, Salesforce"
related: [ECO.M.001, ECO.M.004]
s2r_families: [F4]
---

# ECO.M.005: Оценка рынка — TAM / SAM / SOM

> **Назначение:** Метод оценки размера рынка для стратегии и pitch deck.

---

## 1. Определения

| Метрика | Что измеряет | Вопрос |
|---------|-------------|--------|
| **TAM** (Total Addressable Market) | Весь рынок, если бы у нас было 100% | Насколько велика возможность? |
| **SAM** (Serviceable Addressable Market) | Часть TAM, которую мы можем обслужить (география, сегмент, язык) | Насколько велик наш реалистичный рынок? |
| **SOM** (Serviceable Obtainable Market) | Часть SAM, которую мы реалистично захватим за 3-5 лет | Какова наша реальная цель? |

**Различение:** TAM ≠ Revenue forecast. TAM = ceiling возможности. Revenue forecast = bottom-up projection (ECO.M.001 §8).

---

## 2. Два подхода

### Top-Down (сверху вниз)

```
Глобальный рынок EdTech ($400B)
  → Сегмент: adult professional development ($44B)
    → Подсегмент: online (60%) = $26B
      → География: русскоязычный + англ = TAM
```

**Плюс:** Быстро, использует публичные данные.
**Минус:** Легко раздуть. Инвесторы скептичны к «$100B market × 1%».

### Bottom-Up (снизу вверх) — предпочтительный

```
Количество потенциальных клиентов (ICP)
  × Средний чек (ARPU)
  × Penetration rate
  = SOM → SAM → TAM
```

**Пример для IWE:**
```
ICP: практики с ≥3 лет опыта, интерес к системному мышлению
Русскоязычный рынок: ~200K потенциальных (из ~2M IT-специалистов × 10% fit)
ARPU: $240/год (текущий)
SOM (3 года): 5K платящих × $240 = $1.2M ARR
SAM: 200K × $240 = $48M
TAM (+ англ рынок): 2M × $240 = $480M
```

---

## 3. Валидация

**Best practice:** Применить оба подхода. Если расхождение <15% — допущения надёжны.

**Что проверять:**
- Количество ICP — из census data, LinkedIn, ZoomInfo, собственных данных
- ARPU — из текущих клиентов или comparable companies
- Penetration rate — из аналогов в смежных рынках

---

## 4. Как инвесторы оценивают TAM/SAM/SOM

| Что смотрят | Red flag | Green flag |
|-------------|----------|------------|
| Метод | Только top-down | Bottom-up + top-down cross-check |
| Источники | «По нашим оценкам» | Публичные данные + собственная воронка |
| SOM | >10% SAM за 3 года | 1-5% SAM с обоснованием |
| TAM | <$1B (слишком мал для VC) | $1-10B (seed), $10B+ (Series A+) |
| Growth | Статичный рынок | CAGR >15% |

---

## 5. Failure modes

| ID | Ошибка | Последствие |
|----|--------|-------------|
| FM.TAM.001 | TAM = вся отрасль ($400B EdTech) | Инвестор не верит → «не знает свой рынок» |
| FM.TAM.002 | Нет bottom-up | Нет unit economics → слабый pitch |
| FM.TAM.003 | SOM >10% SAM | Нереалистичные ожидания → down round |
| FM.TAM.004 | Статичный TAM | Нет growth story → «зачем инвестировать?» |
