# 逐字稿閱讀室 · Transcript Desk

A lightweight audio-and-transcript reader/editor. Open an existing Buzz SRT or VTT with its original recording, read along during playback, edit the wording, and save a corrected copy. No transcription service or AI API is required.

## 使用方法

1. 開啟網站，按「開啟錄音」選擇原始錄音。
2. 按「開啟逐字稿」選擇從 Buzz 匯出的 SRT 或 VTT。
3. 按一下句子，從對應時間開始播放；按「編輯」修訂文字，再按「套用」。
4. 按「另存副本」，下載修訂後的 SRT。關閉分頁前，請先儲存修改。

頁首可切換香港繁體中文及 English。介面語言不會翻譯或改動逐字稿內容。

## Features

- SRT/VTT import and timestamp-linked audio playback
- Current-sentence highlighting and optional following
- Playback speed, five-second skip, and sentence looping
- Text editing, undo, and search
- SRT, VTT, timestamped TXT, and project JSON export
- Hong Kong Traditional Chinese and English interfaces
- Light and dark modes; responsive layout

## Privacy and files

Audio and transcript files are opened locally in the browser. This application has no file-upload endpoint, analytics, external scripts, fonts, AI calls, or database. GitHub receives normal requests for the website assets, but the application does not send it your selected recordings or transcript contents.

Edits remain in the tab until you download a copy. SRT/VTT preserve sentence timestamps. Project JSON also records the expected audio filename and playback position, but does not embed the recording. Keep the recording's timeline unchanged. Audio codec support depends on the browser; use Edge/Chrome or an MP3/WAV copy with matching timing if necessary.

## Hosting and offline use

GitHub Pages serves the `docs/` directory from `main`. The `docs/.nojekyll` file disables Jekyll processing. There is no build step or package installation.

Download `docs/index.html` and open it in Edge or Chrome for offline use. Share the HTML, original audio, and SRT together if the recipient needs to review a particular recording.

To update the website, edit `docs/index.html` and push to `main`. Never commit recordings, transcripts, API keys, or project files containing private text.
