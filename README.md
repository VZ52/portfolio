# portfolio

Сайт-визитка с авто-деплоем на GitHub Pages через GitHub Actions.

**Живая версия:** https://vz52.github.io/portfolio/

## Стек

- Чистый HTML + CSS (без фреймворков и сборщиков)
- GitHub Actions для CI/CD
- GitHub Pages — хостинг

## Как работает CI/CD

При каждом `git push` в `main`:

1. GitHub Actions триггерится по событию `push`
2. Workflow `.github/workflows/deploy.yml` поднимает Ubuntu-runner
3. Чекаутит код, упаковывает в Pages-артефакт
4. Деплоит на GitHub Pages
5. Через ~30 секунд изменения видны на сайте

## Локальная разработка

Просто открыть `index.html` в браузере. Никаких npm-команд.

## Автор

Зайцев Константин — https://github.com/VZ52
