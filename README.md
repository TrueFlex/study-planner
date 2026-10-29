# Учебный планировщик студента

[![Deploy static site](https://github.com/TrueFlex/study-planner/actions/workflows/deploy.yml/badge.svg)](https://github.com/TrueFlex/study-planner/actions/workflows/deploy.yml)

Лендинг веб-сервиса, который собирает задания по всем дисциплинам в один список со сроками сдачи. Учебный проект по курсу «Информатика» (ГУАП, 2026): лабораторные работы 4–6.

**Сайт:** https://trueflex.github.io/study-planner/

## Что на странице

- главный экран с ближайшими сроками;
- блоки «Задания приходят из трех мест», «Что будет в первой версии», «Как это работает»;
- интерактивное демо: добавление задания, список по сроку с подсказкой «осталось N дней», отметка о сдаче, фильтр по дисциплине;
- план разработки по этапам и частые вопросы.

Данные демо хранятся только в памяти страницы и никуда не отправляются.

## Технологии

Один файл `index.html`: HTML, CSS и JavaScript без библиотек и внешних шрифтов. Фотографии лежат в папке `images`.

## Как запустить

Открыть `index.html` в браузере или опубликованную версию по ссылке выше.

## Публикация (CI/CD)

Workflow `.github/workflows/deploy.yml` в GitHub Actions:

1. `check` – проверяет `index.html` валидатором html-validate при каждом push и pull request в `main`;
2. `deploy` – после успешной проверки публикует сайт на GitHub Pages, только при push в `main`.

Бейдж вверху показывает результат последнего запуска.

## История работы

| Работа | Что сделано |
| --- | --- |
| ЛР4 | сайт создан по промпту языковой моделью, проверен и исправлен ИИ-агентом (3 правки) |
| ЛР5 | проект выложен на GitHub; в ветках `feature/photos`, `feature/week-view` и `docs/readme` агент добавил фотографии, вид «Неделя» и это описание; ветки объединены с `main` через pull request; сайт опубликован в GitHub Pages |
| ЛР6 | публикация переведена на GitHub Actions (`deploy.yml`), добавлены проверка HTML перед публикацией и бейдж статуса; рассмотрен автодеплой на Vercel |

## Фотографии

Источник – [Pexels](https://www.pexels.com/ru-ru/license/), бесплатная лицензия Pexels:

- `images/student.jpg` – [Yan Krukov](https://www.pexels.com/ru-ru/photo/8199249/);
- `images/desk.jpg` – [Jessica Lewis](https://www.pexels.com/ru-ru/photo/iphone-7-macbook-pro-583846/);
- `images/planner.jpg` – [Bich Tran](https://www.pexels.com/ru-ru/photo/760718/).

---

Учебный демонстрационный проект, не коммерческий сервис.
