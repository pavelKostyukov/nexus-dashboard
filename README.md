# NEXUS — Operations Hub

Личный дашборд: проекты, задачи, YouTube-студия, AI-агенты.

## Changelog

### v2.0.1 — Fix layout: двойная прокрутка и наложение sidebar
- Убрана двойная прокрутка (body + content)
- Sidebar: непрозрачный фон вместо backdrop-filter
- Topbar: position relative вместо sticky
- Фоновые градиенты: z-index -1 вместо 0
- Убран scroll-behavior smooth

### v2.0.0 — Initial release
- Полный дашборд: 9 разделов, 7 проектов, 8 AI-агентов
- Канбан с drag & drop
- YouTube Студия с пайплайном
- Графики на Canvas API
- localStorage persistence

## Запуск
Открыть index.html в браузере. Сборка не нужна.

## Деплой
Скопировать index.html в /var/www/html (nginx) или public_html (apache).
Или GitHub Pages: Settings → Pages → Deploy from branch → main.

## Данные
localStorage браузера. Бэкап: Настройки → Экспорт JSON.

## AI-агенты
По умолчанию демо-режим. Реальный API: Настройки → Endpoint / Model.
Ключ Qwen на публичном сервере хранить только в backend-прокси, не в браузере.

## Модули
- Обзор: KPI, графики, AI-сводка дня
- Проекты: канбан с drag&drop (7 направлений)
- YouTube Студия: пайплайн выпусков, сценарий, чек-лист
- AI Агенты: 8 ролей, чат, демо-режим + настройка Qwen API
- Финансы: цели 60/40 млн, ИИС, ETF, ЖК Дюна
- Ozon: каталог SKU, маржа, остатки, готовность карточек
- Здоровье: метрики, дневник сна, план по апноэ
- Семья: мама и бабушка, лекарства, календарь заботы
- Настройки: API, экспорт/импорт JSON, автоскролл чата