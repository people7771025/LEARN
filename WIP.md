# WIP — LEARN 教學系統入口

最後更新：2026-07-03（台北時間）/ Claude

## 現在狀態

- 單檔 `index.html`，離線可開；GitHub Pages：<https://people7771025.github.io/LEARN/>
- 本輪完成全站體檢＋五項優化（已驗證、已推送）：
  - 手機重排：側欄精簡（645→272px），第一屏即見課程卡（原本要滑到 1467px）
  - 互動補完：選卡後焦點保留、無選課時複製鈕停用、空狀態一鍵重置、隱藏篩選捲軸
  - 門面：計數改「N 套」、LANG 狀態改「完成」（線上版已部署）、SVG favicon、meta/og/theme-color
  - 選課記憶：localStorage `learn.entry.v1`（只存 LEARN 自己的 selected+filter）
  - 無障礙：卡片標題改真按鈕＋整卡覆蓋層、移除多餘 aria-live、手機觸控 44px+
- Playwright 全流程驗證：桌機/手機/320px/深色/焦點/持久化/複製 toast 全過，console 0 錯誤。
- ⚠️ **線上版尚未部署成功**：`f4a95a5` 推送後 GitHub Pages 連三次失敗（建置成功、部署卡 `deployment_queued` 10 分鐘逾時；GitHub 狀態頁無事故，repo 內容無問題）。線上仍是 6/25 舊版，功能正常。下一步：再觸發部署（push 即觸發）；若持續失敗，考慮 Pages 停用再啟用（需使用者同意）。

## 下一步

1. 新教學專案：在 `COURSES` 陣列加一筆即可（見 HANDOFF）。
2. 跨專案進度同步刻意不做，避免破壞各專案獨立性。

## 卡點

- 無卡點。
