# AGENTS.md — talking-type-releases

先讀 [`docs/HANDOFF.md`](docs/HANDOFF.md)。本 repo 目前沒有 `CURRENT_TASK` 規格檔。不要在本公開 repo 放原始碼或憑證。

## 交接協議（所有 AI 必守）

任何更動——程式、檔案或資料夾的新增／刪除／搬移／改名、設定、規則、skill、分支或 PR 狀態、與部署有關的現況——在結束本次工作或 commit 之前，必須在 `docs/HANDOFF.md` 追加一筆交接紀錄。

每筆固定寫：編號（H-001、H-002…）、時間（Asia/Taipei）、哪個 AI、分支與 commit、改了什麼（含搬移或新增的路徑）、目前狀態、下一步、卡住的地方或需要 Angus 核准的事項。

滿 5 筆為一輪：把這 5 筆摺進本檔檔首「目前狀態」摘要，把原文移到 `docs/handoff/archive/HANDOFF-H00x-H00y.md`，讓本檔保持精簡。不要刪歷史。

任何待辦、checklist 或任務清單：完成一項且已寫好對應的 H-xxx 交接紀錄後，直接刪掉該項，不要打勾留著。清單空了就刪除整個檔案與所有指向它的一行，並在 `docs/HANDOFF.md` 記一筆。

本協議不取代既有流水線。規格、測試、`verify.sh`、`review_cli.mjs`、merge 與發布規則仍以 `~/Deving/agent-governance/docs/DIVISION_OF_LABOR.md` 為準。

## 本 repo 特別的地方

- 這是 Talking-Type 的**公開**發行 repo：只放已簽署、公證的下載檔、更新檔與使用說明，不放原始碼。原始碼在私有的 [`Talking-Type`](https://github.com/angus-song-admin/Talking-Type)。
- Issues 與 wiki 已關閉。不要把原始碼、憑證或未公證的檔案推進本 repo。
- App 內更新讀 `https://api.github.com/repos/angus-song-admin/talking-type-releases/releases/latest`。

- 不要讀、寫、印出 `.env*` 或任何金鑰。
- 不要直推預設分支，不要改寫歷史，不要刪遠端分支。
- merge、發布與任何正式簽署／公證，都要 Angus 明確同意。
