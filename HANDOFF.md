# HANDOFF — LEARN 教學系統入口

## 專案定位

- 單檔 HTML：`index.html`
- 離線可開、無 build step、無 npm
- 主題：FIN / OPT / LANG 的統一入口
- 狀態：無跨專案資料同步；只做選課與導覽

## 檔案

- `index.html`：主頁、CSS、JS、課程資料全在單檔
- `README.md`：使用說明
- `WIP.md`：目前狀態與下一步
- `HANDOFF.md`：交接資訊

## 課程資料

入口資料集中在 `COURSES`：

```js
{
  id,
  code,
  title,
  subtitle,
  category,
  categoryLabel,
  color,
  localUrl,
  onlineUrl,
  scope,
  hours,
  status,
  routes,
  outcome,
  tags,
  steps
}
```

新增教學專案時：

1. 在 `$HOME/Dev/<PROJECT>` 建立可開啟的 `index.html`
2. 在 `COURSES` 增加一筆
3. 若有線上版，填 `onlineUrl`
4. 更新 README / WIP

## 目前入口

- FIN：`../FIN/index.html`，線上版 `https://people7771025.github.io/FIN/`
- OPT：`../OPT/index.html`，線上版 `https://people7771025.github.io/OPT/`
- LANG：`../LANG/index.html`，目前無線上版

## 注意

- 不要把 FIN / OPT / LANG 的課程內容複製進 LEARN。
- LEARN 不讀取其他專案的 localStorage，避免不同 origin 或部署方式造成不穩定。
- 如果要讓各專案都有「回入口」按鈕，建議在各專案單獨加一個相對連結到 `../LEARN/index.html`，並分別 commit。
