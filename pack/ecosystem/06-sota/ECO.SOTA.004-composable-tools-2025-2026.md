---
id: ECO.SOTA.004
title: "Composable Architecture & Low-Code/No-Code Ecosystem Tools (2025-2026)"
type: sota
status: active
created: 2026-03-24
source: "Gartner Composable Business, Hiper No-Code 2026, WeWeb Low-Code Guide, JRDSI AI-Powered LCNC, McKinsey LCNC Survey 2025, DEVOPSdigest LCNC Predictions 2026"
related: [ECO.M.008, ECO.M.009, ECO.M.007]
s2r_families: [F8]
---

# ECO.SOTA.004: Composable Architecture & Low-Code/No-Code Tools (2025-2026)

## Контекст

К 2026 году границы между no-code, low-code и pro-code размываются — AI становится связующим слоем. 71% предприятий с LCNC-платформами сократили время разработки на 50%+ (McKinsey 2025). К 2026 году 80% пользователей low-code — не-IT-специалисты (Gartner).

---

## Composable Architecture

**Принцип:** Экосистема строится из модульных, переиспользуемых компонентов, соединённых через API. Каждый компонент может быть заменён без перестройки целого.

### Три уровня composability

| Уровень | Что собирается | Кто собирает | Пример (IWE) |
|---------|---------------|-------------|---------------|
| **Composable Business** | Бизнес-capabilities | Стратег (F7, F4) | Методология + AI + Сообщество |
| **Composable Platform** | Технические компоненты | Архитектор (F5, F8) | LMS + Ory + Neon + Bot |
| **Composable UX** | UI-блоки и workflows | Дизайнер + AI | Персонализированный learning path |

---

## Конвергенция No-Code / Low-Code / Pro-Code

### Спектр 2026

| Уровень | Кто | Инструменты | Применение |
|---------|-----|-------------|------------|
| **No-code** | Domain experts, менеджеры | Zapier, Make, Notion, monday.com | Workflows, формы, дашборды |
| **Low-code** | Citizen developers, аналитики | OutSystems, Mendix, Power Apps, Retool | Внутренние apps, CRUD, интеграции |
| **Pro-code** | Инженеры | VS Code, GitHub, Railway, Vercel | Core platform, API, complex logic |
| **AI-assisted** | Все | Cursor, Claude Code, Copilot | Генерация из описания на естественном языке |

### Тренд: AI как связующий слой

Маркетинг-менеджер описывает workflow на естественном языке → AI генерирует → no-code платформа исполняет. Разработчик описывает API → AI генерирует код + тесты + документацию.

---

## Ведущие платформы (2025-2026)

| Платформа | Фокус | Релевантность для IWE |
|-----------|-------|----------------------|
| **Retool** | Internal tools, admin panels | Админка для LMS |
| **WeWeb + Supabase** | Frontend + backend (visual) | Landing, user dashboard |
| **n8n / Make** | Workflow automation | Интеграционные цепочки (бот → LMS → email) |
| **Creatio** | CRM + process automation | Студент journey, sales pipeline |
| **OutSystems** | Enterprise apps | Если масштаб enterprise |

---

## Паттерны применения в EdTech

| Паттерн | Описание | Преимущество |
|---------|----------|-------------|
| **API-first + no-code orchestration** | Core на pro-code, workflows на no-code | Скорость итераций без потери контроля |
| **Internal Developer Portal** | Backstage/Port: каталог сервисов, docs, templates | Снижение onboarding time |
| **Event-driven LCNC** | Триггеры (webhook) → no-code обработка | Non-engineers реагируют на события |
| **AI agent builder** | No-code создание агентов поверх LLM API | Менторы создают своих ботов |

---

## Ключевые метрики LCNC

| Метрика | Benchmark 2025 |
|---------|---------------|
| Time-to-first-app | <1 день (no-code), <1 неделя (low-code) |
| Reduction in dev time | 50-70% (McKinsey) |
| Citizen developer adoption | 80% пользователей LCNC — не-IT (Gartner 2026) |
| Maintenance cost reduction | 40-60% vs custom code |

---

## Ключевые выводы для IWE

1. **Pro-code для ядра** (методология, Digital Twin, Agent SDK), **no-code для workflows** (уведомления, onboarding, интеграции)
2. **n8n/Make** — кандидаты для автоматизации рутинных цепочек (бот → email → LMS sync)
3. **Retool** — кандидат для admin panels и внутренних инструментов
4. **AI agent builder** — стратегическая возможность: менторы создают агентов без кода → ecosystem effect
5. **Internal Developer Portal** — нужен при масштабировании команды (>3 разработчиков)
