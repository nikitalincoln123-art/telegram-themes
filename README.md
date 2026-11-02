# TGThemes — каталог тем и плагинов для Telegram

Статический каталог кастомных тем (`.attheme`) и плагинов (`.plugin`) для Telegram, ExtraGram и AyuGram.

## Возможности

- Живое превью темы прямо на главной — клик по теме окрашивает экран-имитацию чата
- 5 готовых тем `.attheme` для скачивания
- Стартовый шаблон плагина (`starter-template.plugin` + исходник `.plugin.py`) для ExtraGram/AyuGram
- Секция «Как установить»

## Структура

```
├── index.html          # главная (hero, живое превью, плагины, как установить)
├── themes.html         # каталог тем
├── plugins.html        # каталог плагинов
├── css/style.css       # стили
├── images/             # превью-скриншоты тем
├── themes/             # файлы тем .attheme
└── plugins/            # файлы плагинов .plugin
```

## Деплой на GitHub Pages

Сайт использует относительные пути, поэтому работает из подпапки (project Pages).

Опубликовано автоматически через GitHub Actions (workflow `static.yml`).