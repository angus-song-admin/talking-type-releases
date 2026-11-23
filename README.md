# Talking-Type

English ｜ [繁體中文](README.zh-TW.md)

Always-on voice typing for macOS (Apple Silicon, macOS 14+). Leave it running in the menu bar and whatever you say is typed into the text field of the app you're using.

**[Download Talking-Type.dmg](https://github.com/angus-song-admin/talking-type-releases/releases/latest/download/Talking-Type.dmg)** — drag it into Applications and open it. The first launch walks you through permissions and downloads the on-device speech model (about 180 MB, once).

This repository only hosts signed, notarized downloads and in-app updates. The app only installs an update signed by the same developer and accepted by Gatekeeper.

## What it does

- **Voice typing**: after each sentence, the transcript is typed where your cursor is.
- **AI cleanup (optional, your own key)**: after each passage, filler words and false starts are removed, lists are formatted and the tone matches the app.
- It only types into text fields. It never clicks buttons, sends messages or operates apps for you.

## Where your data goes

- **On-device transcription** (default): audio never leaves your Mac.
- **OpenAI transcription** (optional, your own key): audio of detected speech goes to OpenAI.
- **AI cleanup** (optional, your own OpenAI or Claude key): the transcript plus up to 400 characters around the cursor, the selected text, up to about 1,500 characters of visible window text, the app name, window title and URL go to the provider you chose.
- Keys are stored in the macOS Keychain. Local history is off by default; logs are readable only by you.

## Permissions

Microphone; Accessibility (to paste); Screen Recording (optional, only to read on-screen text in apps whose text isn't accessible, such as LINE; screenshots stay in memory on your Mac).

## License

Talking-Type is maintained by ICANSTron and derived from the MIT-licensed [urusaqqrun/jarvis-voice](https://github.com/urusaqqrun/jarvis-voice). The on-device model comes from [k2-fsa/sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) ([FunASR model license](https://github.com/modelscope/FunASR?tab=readme-ov-file#license)).
