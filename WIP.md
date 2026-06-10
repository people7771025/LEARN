# WIP — LEARN 教學系統入口

最後更新：2026-06-10（台北時間）/ Codex

## 現在狀態

- 新專案 `$HOME/Dev/LEARN` 已建立，本機 git repo：`main`，目前尚未設定 remote。
- 單檔 `index.html`，離線可開。
- 已納入三個教學系統：
  - FIN：財報判讀
  - OPT：期權/期貨
  - LANG：美語/日語考試
- 功能：
  - 搜尋
  - 目標篩選
  - 課程卡片
  - 選定課程詳細路線
  - 本機/線上入口連結
  - Markdown 路線匯出

## 驗證

- `node` 抽出 `<script>` 後 parser OK。
- 確認三個入口連結存在：
  - `../FIN/index.html`
  - `../OPT/index.html`
  - `../LANG/index.html`
- Playwright 透過臨時本地 server 驗證：
  - 首頁渲染 3 個教學系統、4 個篩選。
  - 搜尋「日檢」可命中 LANG。
  - 篩選「交易風控」可命中 OPT 並同步詳情。
  - Markdown 路線匯出可產生 OPT 內容。
  - 桌面與手機版畫面無明顯重疊。

## 下一步

1. 若未來新增教學專案，將該專案加到 `COURSES` 陣列。
2. 若要部署，建立 GitHub remote 後推送並啟用 GitHub Pages。
3. 若要跨專案同步進度，需要先統一 localStorage key 或改為後端儲存；目前刻意不做，避免破壞各專案獨立性。

## 卡點

- 無 remote，暫時只能本機 commit，不能 push。
