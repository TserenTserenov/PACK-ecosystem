# spf-ecosystem-pack

> **Тип репозитория:** `Pack`

> Pack (паспорт области) для предметной области «Экосистема развития интеллекта»

## Что это

Это **source-of-truth** для области «Экосистема развития интеллекта» — связанной совокупности ресурсов, сервисов и сообществ, обеспечивающих бесшовный путь развития от первого знакомства до системного мышления мирового уровня.

## Тип репозитория

- **Тип**: Pack
- **Source-of-truth**: Да
- **Область**: Экосистема развития интеллекта

## Структура

```
spf-ecosystem-pack/
├── README.md
├── REPO-TYPE.md
└── pack/
    └── ecosystem/
        ├── 00-pack-manifest.md        # Метаданные pack'а
        ├── 01-domain-contract/        # Контракт домена
        │   ├── 01A-bounded-context.md
        │   └── 01B-distinctions.md
        ├── 02-domain-entities/        # Сущности домена
        ├── 03-methods/                # Методы оценки
        ├── 04-work-products/          # Рабочие продукты
        ├── 05-failure-modes/          # Типовые ошибки
        ├── 06-sota/                   # SoTA-аннотации
        └── 07-map/                    # Карты связей
```

## Ключевые понятия

| Понятие | Описание |
|---------|----------|
| **Экосистема** | Связанная система компонентов для развития интеллекта |
| **Бесшовность** | Отсутствие барьеров между компонентами |
| **Компонент** | Ресурс/сервис/сообщество в экосистеме |
| **Путь развития** | Траектория через компоненты |

## Upstream

- [TserenTserenov/SPF](https://github.com/TserenTserenov/SPF) — Second Principles Framework
- [ailev/FPF](https://github.com/ailev/FPF) — First Principles Framework

## Downstream

- [ecosystem-development](https://github.com/aisystant/ecosystem-development) — управление экосистемой

## Non-goals

- НЕ содержит контента курсов
- НЕ описывает ИТ-реализацию (см. spf-digital-platform-pack)
- НЕ описывает персональное развитие (см. spf-personal-pack)

---

*Pack построен по SPF (Second Principles Framework)*
