<p align="center">
  <img src=".github/shadowgram.png" width="128" height="128" alt="Shadowgram">
</p>

<h1 align="center">Shadowgram Desktop</h1>

<p align="center">
  Клиент Telegram для Windows из семейства Shadowgram.<br>
  <a href="https://github.com/andrygasanov-netizen/shadowgram">iPhone</a> ·
  <a href="https://github.com/andrygasanov-netizen/shadowgram-android">Android</a> ·
  <a href="#english">English</a>
</p>

> Shadowgram Desktop — форк [AyuGram Desktop](https://github.com/AyuGram/AyuGramDesktop), который построен на официальном
> [Telegram Desktop](https://github.com/telegramdesktop/tdesktop). Не связан с Telegram FZ-LLC и AyuGram.

## Состояние

Сейчас это сборка AyuGram Desktop под Windows x64 через GitHub Actions. Собственных функций Shadowgram в десктопной версии пока нет, а готовых релизов ещё не выкладывалось. Всё, что описано ниже, умеет AyuGram Desktop.

Функции мобильного Shadowgram (Shadowgram Tools, скрытые чаты, автопрокси и другие) есть в версиях для [iPhone](https://github.com/andrygasanov-netizen/shadowgram) и [Android](https://github.com/andrygasanov-netizen/shadowgram-android).

## Возможности

- **Режим призрака** с гибкой настройкой: без «прочитано», «печатает…», «в сети», скрытый просмотр историй.
- **История сообщений:** удалённые и отредактированные сообщения остаются видны.
- **Анти-удаление** (anti-recall).
- Настройка шрифтов.
- **Режим стримера:** скрывает приложение от захвата экрана.
- Локальный Telegram Premium (только оформление на вашем устройстве).
- Встроенный переводчик.
- Расширенные настройки внешнего вида.

Подробное описание функций — в [документации AyuGram](https://docs.ayugram.one/desktop/).

## Сборка под Windows

Сборка идёт в GitHub Actions: workflow **Build Ugram Desktop (Windows x64)** (`.github/workflows/ugram-win.yml`), запуск вручную.

```sh
gh workflow run ugram-win.yml -R andrygasanov-netizen/shadowgram-desktop
```

Сборка долгая (несколько часов): она собирает Qt и все библиотеки Telegram Desktop. Готовый файл появится в артефактах запуска.

Собрать локально можно по [руководству AyuGram](https://github.com/AyuGram/AyuGramDesktop/blob/dev/docs/building-win-x64.md).

## Лицензия и благодарности

Код распространяется под лицензией **GNU GPL v3**, как Telegram Desktop и AyuGram.

- [Telegram Desktop](https://github.com/telegramdesktop/tdesktop)
- [AyuGram Desktop](https://github.com/AyuGram/AyuGramDesktop) — основа этой сборки и все функции, описанные выше.
- [Kotatogram](https://github.com/kotatogram/kotatogram-desktop) и другие клиенты, на которые опирается AyuGram.

---

<a id="english"></a>

# Shadowgram Desktop (English)

A Telegram client for Windows from the Shadowgram family. A fork of [AyuGram Desktop](https://github.com/AyuGram/AyuGramDesktop), which is built on the official [Telegram Desktop](https://github.com/telegramdesktop/tdesktop). Not affiliated with Telegram FZ-LLC or AyuGram.

## Status

For now this is an AyuGram Desktop build for Windows x64 made with GitHub Actions. The desktop version has no Shadowgram features of its own yet, and no releases have been published. The features below come from AyuGram Desktop. Shadowgram's own features (Shadowgram Tools, hidden chats, auto proxy and more) are in the [iPhone](https://github.com/andrygasanov-netizen/shadowgram) and [Android](https://github.com/andrygasanov-netizen/shadowgram-android) apps.

## Features

Flexible ghost mode, message history (deleted and edited messages stay visible), anti-recall, font customization, streamer mode, local Telegram Premium, a translator and an enhanced appearance. See the [AyuGram documentation](https://docs.ayugram.one/desktop/).

## Build

GitHub Actions workflow **Build Ugram Desktop (Windows x64)** (`.github/workflows/ugram-win.yml`), manual run. The build takes several hours; the result is in the run's artifacts. For a local build, follow the [AyuGram guide](https://github.com/AyuGram/AyuGramDesktop/blob/dev/docs/building-win-x64.md).

## License

GNU GPL v3, like Telegram Desktop and AyuGram. Thanks to [Telegram Desktop](https://github.com/telegramdesktop/tdesktop), [AyuGram Desktop](https://github.com/AyuGram/AyuGramDesktop) and [Kotatogram](https://github.com/kotatogram/kotatogram-desktop).
