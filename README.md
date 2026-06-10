# LEARN 教學系統入口

統一入口頁，集中導覽目前的教學專案：

- `FIN`：台股/美股財報判讀自學系統
- `OPT`：美股期權 + 台股期貨自學系統
- `LANG`：美語/日語考試自學系統

## 怎麼用

1. 直接打開 `index.html`
2. 用左側搜尋或目標篩選選擇想學的主題
3. 點「開啟課程」進入對應專案

入口頁使用相對連結：

- `../FIN/index.html`
- `../OPT/index.html`
- `../LANG/index.html`

因此建議直接從檔案系統開啟 `LEARN/index.html`。

## 線上版

入口網址：

- <https://people7771025.github.io/LEARN/>

課程固定網址：

- FIN：<https://people7771025.github.io/FIN/>
- OPT：<https://people7771025.github.io/OPT/>
- LANG：<https://people7771025.github.io/LANG/>

## 範圍

- 選課與導覽
- 依目標篩選：投資分析、交易風控、語言考試
- 顯示每個系統的學習範圍、時間、建議路線
- 匯出選定路線為 Markdown

## 注意

- LEARN 不搬移各專案內容，也不讀取各專案 localStorage。
- 各課程進度仍由 FIN / OPT / LANG 自己保存。
- 單檔 HTML，無 build step、無套件安裝。
