# 交接紀錄：talking-type-releases（公開發行檔）

> 所有 AI（Claude Code、Codex、Antigravity／agy、Grok Bot）**每次開工先讀本檔**。本 repo 目前沒有 `CURRENT_TASK` 規格檔；需要時再依 `~/Deving/agent-governance/templates/CURRENT_TASK.md` 新增，且不得取代本檔。

## 交接協議（所有 AI 必守）

任何更動——程式、檔案或資料夾的新增／刪除／搬移／改名、設定、規則、skill、分支或 PR 狀態、與部署有關的現況——在結束本次工作或 commit 之前，必須在 `docs/HANDOFF.md` 追加一筆交接紀錄。

每筆固定寫：編號（H-001、H-002…）、時間（Asia/Taipei）、哪個 AI、分支與 commit、改了什麼（含搬移或新增的路徑）、目前狀態、下一步、卡住的地方或需要 Angus 核准的事項。

滿 5 筆為一輪：把這 5 筆摺進本檔檔首「目前狀態」摘要，把原文移到 `docs/handoff/archive/HANDOFF-H00x-H00y.md`，讓本檔保持精簡。不要刪歷史。

本協議不取代既有流水線。規格、測試、`verify.sh`、`review_cli.mjs`、merge 與發布規則仍以 `~/Deving/agent-governance/docs/DIVISION_OF_LABOR.md` 為準。

## 目前狀態

- **公開** repo。預設分支 `main` `451c6e4`（2026-11-23 22:48）：中英文下載頁與使用說明。前一筆是 Initial commit `e5a21b7`（22:45）。只有 `README.md`、`README.zh-TW.md` 兩個檔。只有 `main` 一條分支。
- 盤點時沒有 GitHub Release（`gh release list` 為 0）。Issues 已停用。無 GitHub Actions。無開著的 PR。

## 最近紀錄

### H-001

- **時間**：2026-11-25 17:35（Asia/Taipei）
- **AI**：Grok Bot
- **分支／commit**：`main` `451c6e4`（盤點時的預設分支 HEAD）
- **變更**：唯讀盤點 GitHub 現況，無程式變更。盤點原文：雲端 box `/workspace/handoff/AGENT_HANDOFF.md`（不在本 repo）。
- **目前狀態**：說明文件已在 main。尚未有實際 Release 資產。
- **下一步**：發第一個版本前，先在私有 Talking-Type repo 用 Developer ID 打包與公證，再由 Angus 把檔案放到本 repo 的 Release。不要在本 repo 放原始碼。
- **卡住／需 Angus 核准**：建立公開 Release、簽署與公證，都要 Angus 處理或同意。

### H-002

- **時間**：2026-11-25 17:45（Asia/Taipei）
- **AI**：Grok Bot
- **分支／commit**：`docs/handoff-protocol`（SHA 於 commit 後填入）
- **變更**：新增所有 AI 共用的交接協議與入口。新增或修改的路徑：
  - 新增 `docs/HANDOFF.md`、`AGENTS.md`、`CLAUDE.md`、`GEMINI.md`、`docs/handoff/archive/README.md`
- **目前狀態**：協議已寫在本分支，尚未合併。未跑 `review_cli.mjs`。未發布。
- **下一步**：經 Angus 同意後審查、合併本 PR。後續任何更動繼續追加 H-003 起。
- **卡住／需 Angus 核准**：合併本分支、發布（若適用）都要 Angus 同意。
