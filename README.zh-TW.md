# Talking-Type

[English](README.md) ｜ 繁體中文

macOS 自動語音輸入（Apple Silicon、macOS 14 以上）。開著放在選單列，你講的話直接寫進正在用的 app 的輸入框。

**[下載 Talking-Type.dmg](https://github.com/angus-song-admin/talking-type-releases/releases/latest/download/Talking-Type.dmg)**，把 Talking-Type 拖進「應用程式」打開。第一次打開會帶你開權限、下載本機辨識模型（約 180 MB，只要一次）。

這個 repo 只放簽好、公證過的下載檔與 App 內更新。App 只會換成同一個開發者簽章、Gatekeeper 認得的新版。

## 做什麼

- **語音輸入**：講完一句，轉出來的字寫進游標所在的輸入框。
- **AI 整理**（選用，用你自己的 key）：講完一段，去贅字、改口只留結果、排條列、依 app 調語氣。
- 只會把字寫進輸入框，不會替你點按鈕、送出訊息或操作 app。

## 資料送去哪

- **本機辨識**（預設）：聲音不離開你的電腦。
- **OpenAI 轉寫**（選用，你自己的 key）：判定是人聲的片段送到 OpenAI。
- **AI 整理**（選用，你自己的 OpenAI 或 Claude key）：轉寫稿，加上游標前後各最多 400 字、選取的字、視窗裡看得到的字（最多約 1,500 字）、app 名稱、視窗標題、網址，送到你選的那家。
- key 存在 macOS 鑰匙圈。本機歷史預設關；log 只有你自己讀得到。

## 權限

麥克風；輔助使用（貼上要用）；螢幕錄影（選用，只有讀不到畫面文字的 app，例如 LINE，才截圖認字；截圖只在記憶體裡、在你的電腦上處理）。

## 授權

Talking-Type 由 ICANSTron 維護，改自 MIT 授權的 [urusaqqrun/jarvis-voice](https://github.com/urusaqqrun/jarvis-voice)。本機模型來自 [k2-fsa/sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx)（[FunASR 的模型授權條款](https://github.com/modelscope/FunASR?tab=readme-ov-file#license)）。
