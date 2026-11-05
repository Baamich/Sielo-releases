# Sielo

Лёгкое приложение для эфиров и записи на Windows. [English below](#english)

**[Скачать установщик](https://github.com/Baamich/Sielo-releases/releases/latest/download/SieloSetup.exe)** · [Все версии](https://github.com/Baamich/Sielo-releases/releases)

## Установка

1. Скачайте и запустите `SieloSetup.exe`. Права администратора не нужны.
2. Выберите папку и версию, по умолчанию стоит последняя.
3. Дальше обновления приходят сами: программа предлагает их при запуске и проверяет подпись каждого.

Если вы переходите с Sielo 0.1.0, сцены и настройки скопируются в новую папку, а оригиналы останутся на месте.

Установщик пока без подписи разработчика, поэтому Windows может показать предупреждение SmartScreen. Чтобы продолжить, нажмите «Подробнее» и «Выполнить в любом случае».

## Что умеет

- **Эфир и запись:** несколько площадок сразу, автобитрейт, задержка эфира, запись частями, HEVC, отдельные дорожки каналов, повтор последних секунд.
- **Сцены:** группы, режим студии, мультивью, переходы, в том числе роликом с прозрачностью.
- **Источники:** экран, окно, игра без внедрения в процесс, камера, страница, видео и списки видео, картинки, слайд-шоу, текст, чат.
- **Звук:** микшер, шумодав, компрессор, лимитер, эквалайзер, приглушение музыки голосом, плагины VST3.
- **Чат в кадре без браузера:** Twitch и PartyWatcher, со смайлами.
- **Виртуальная камера и микрофон:** кадр и звук для Discord, Zoom и VDO.Ninja. Для микрофона нужен установленный виртуальный кабель, например VB-CABLE.
- **Управление:** горячие клавиши, Stream Deck и Streamer.bot по протоколу obs-websocket, скрипты на Lua, автозапуск эфира.
- **Переход с OBS:** импорт сцен, источников и фильтров. Окно импорта заранее показывает, что именно не перенесётся.
- **Экономия:** когда кадр никому не нужен, программа почти не тратит процессор и видеокарту.

## Требования

- Windows 10 или 11, 64 бита.
- Для страниц нужен Microsoft Edge WebView2. Если его нет, установщик поставит его сам.

## Состояние

Это ранняя версия. Основная проверка шла на Windows 10 с видеокартой NVIDIA. Видеокарты AMD и Intel, а также эфир на отдельные площадки проверены меньше. Если что-то не работает, приложите файл из «Справка → Открыть папку с логами».

## Лицензии

Здесь только готовые сборки. В Sielo используется FFmpeg под лицензией LGPL: его исходники лежат в каждом выпуске (`ffmpeg-source-*.zip`), остальные компоненты перечислены в `THIRD_PARTY.txt` рядом с программой. Sielo не связан с OBS Project, Twitch, VB-Audio и другими упомянутыми компаниями.

---

## English

Sielo is a lightweight streaming and recording app for Windows.

**[Download the installer](https://github.com/Baamich/Sielo-releases/releases/latest/download/SieloSetup.exe)** · [All versions](https://github.com/Baamich/Sielo-releases/releases)

1. Run `SieloSetup.exe`. No administrator rights are needed.
2. Choose a folder and a version. The latest one is selected by default.
3. Updates are offered at launch, and each one has its signature checked.

The installer has no developer signature yet, so Windows may show a SmartScreen warning. To continue, choose "More info" and "Run anyway".

**Features:** streaming to several platforms at once, recording, scenes and groups, studio mode, multiview, transitions, game capture without injection, audio filters and VST3 plugins, chat in the frame without a browser, virtual camera, virtual microphone through an installed audio cable such as VB-CABLE, hotkeys, Stream Deck and Streamer.bot through the obs-websocket protocol, Lua scripts, automatic stream start, and scene import from OBS that shows exactly what does not carry over.

**Requirements:** 64-bit Windows 10 or 11. Pages need Microsoft Edge WebView2, and the installer adds it if it is missing.

**Status:** this is an early version, tested mainly on Windows 10 with an NVIDIA graphics card. AMD and Intel graphics cards and streaming to individual platforms have had less testing.

**Licenses:** this repository holds builds only. Sielo uses FFmpeg under the LGPL: its source is attached to every release (`ffmpeg-source-*.zip`), and other components are listed in `THIRD_PARTY.txt` next to the program. Sielo is not affiliated with the OBS Project, Twitch, VB-Audio or other companies mentioned here.
