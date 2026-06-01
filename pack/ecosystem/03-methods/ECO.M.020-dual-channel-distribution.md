---
id: ECO.M.020
name: Dual-channel distribution
type: method
domain: ECO
status: draft
valid_from: 2026-05-27
source_session: peer-сессия 21 (wp358-archgate, Тема 2 mitigation)
---

# ECO.M.020: Dual-channel distribution — marketplace + side-load fallback против single-vendor lock

## Контекст

Marketplace'ы (Microsoft VS Code, Chrome Web Store, Apple App Store, npm, Slack App Directory, GitHub Apps) — single point of failure для extension/plugin/app разработчиков:
- Мораторий на публикации (политика безопасности).
- Удаление аккаунта (false-positive автоматического review).
- Смена политики дистрибуции (платная подписка, новые требования).

Любое из этих событий ломает доставку обновлений действующим пользователям.

## Алгоритм

1. **Основной канал.** Публикация через marketplace (VS Code Extension Marketplace, Chrome Web Store, etc.).
2. **Backup-канал — обязательный.** CI pipeline дополнительно собирает и публикует side-load artifact:
   - VS Code: `.vsix` файл.
   - Chrome: `.crx` или unpacked.
   - iOS: TestFlight / ad-hoc IPA.
   - npm: tarball на собственном CDN.
3. **Distribution backup artifact'а.**
   - GitHub release (signed, versioned).
   - Собственный домен с changelog + install instructions.
   - Документация по side-load — часть README, не «когда понадобится».
4. **CI-автоматизация.** Backup публикуется автоматически на каждом релизе, не вручную при кризисе.

## Стоимость

~4-8 часов дополнительной работы на extension/plugin на этапе первого релиза. Поддержка — нулевая (CI делает всё).

## Граница применимости

**Применять, когда:**
- Marketplace — единственный официальный канал доставки обновлений.
- Есть действующие пользователи, для которых разрыв доставки → потеря данных / рабочего процесса.
- Marketplace-policy непрозрачна или менялась за последние 2 года.

**Анти-паттерн:** «Когда заблокируют — придумаем.» Поздно: у нас уже live-зависимые пользователи. Backup-канал — превентивная, не реактивная мера.

## Применимость

VS Code, Chrome, Firefox, Slack, GitHub Apps, mobile app stores, npm / PyPI / RubyGems, любые extension/plugin/app системы с marketplace-зависимостью.

## Источник

Peer-сессия 21 «wp358-archgate» (2026-05-27), Тема 2 mitigation.
