# mywebsite — 離線 HTML 工具集

> GitHub: https://github.com/newsprout1013/mywebsite
> 部署方式：**GitHub Pages**，push main 即上線（實測約 30 秒 CDN 更新完成）
> 線上網址：`https://newsprout1013.github.io/mywebsite/<檔名>.html`
> ⚠️ 這是 **public** repo，寫進檔案的內容都會公開，勿放個資或金鑰

---

## 專案概述

這個 repo 放的是阿翰自用的**離線單機 HTML 工具**，每個檔案是獨立的單頁應用，主要在手機瀏覽器使用。

| 檔案 | 用途 | 附屬檔 |
|------|------|--------|
| `dabeizhan_practice.html` | 千手眼大悲心咒行法・修持（研修營筆記＋十科儀軌＋Q&A，43 頁翻頁式） | `manifest.json`、`sw.js`、`icon-*.png`、`apple-touch-icon.png` |
| `dabeizhan.html` | 千手眼大悲心咒行法（儀軌全文，捲動式） | — |
| `choujian.html` | 佛法法語抽籤 | `choujian-manifest.json`、`choujian-*.png` |
| `zhunian_clock_F.html` | 助念小工具 | — |
| `health.html` | 天心中醫 健康手冊 | — |
| `Tools.html` | 帳務資料整理小工具 | — |
| `tzuchi-bnt-vaccine.html` | 慈濟 BNT 疫苗採購案：正反解讀與治理啟示 | — |

---

## 開發規則

- 一律**繁體中文**
- 這些都是離線使用的單一 HTML 檔，所有 CSS / JS 內嵌，不依賴外部資源
- `<head>` 必須同時寫兩行 charset（公司舊瀏覽器相容）：
  ```html
  <meta charset="UTF-8">
  <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  ```
- 手機使用為主，注意觸控操作、字級可調、防誤觸
- 經文類頁面使用「捲動感知 + 聰明繼續」模式（詳見 `27-CLAUDE/200_Reference/offline-html-dev-notes.md`）

---

## Git 操作

- 提交身分已在本機設定好（`git config --local user.name / user.email`），不用再設
- 直接在 main 上工作，push 即部署
- 提交訊息用中文，簡述改了什麼

---

## 進度與紀錄

詳見 [PROGRESS.md](PROGRESS.md)
