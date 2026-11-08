# 個人中藥開單紀錄、佣金及數據分析系統 (PWA 離線版)

本專案為純前端離線漸進式網頁應用（PWA），支援上傳至 GitHub Pages 生成 HTTPS 網址，並透過手機或電腦瀏覽器安裝至主畫面，在**完全無網絡（離線）**環境下完整使用所有功能。

## 📁 檔案結構清單

請將以下檔案一併上傳至你的 GitHub Repository 根目錄：

1. `index.html` — 主頁面結構
2. `styles.css` — 介面樣式表
3. `app.js` — 核心邏輯（開單、月曆、改單、全單/部分退款、拍照、數據分析、匯出匯入）
4. `manifest.json` — PWA 安裝設定檔（支援「加入主畫面 / 安裝應用程式」全螢幕獨立執行）
5. `sw.js` — Service Worker 離線快取引擎（首次開啟後自動將所有檔案保存於本地，斷網亦可正常開啟）
6. `icon-192.png` & `icon-512.png` — 手機主畫面應用程式圖示

## 🚀 上傳至 GitHub 並生成 HTTPS 網址步驟

1. 登入 GitHub，點擊右上角 **+** 號選擇 **New repository**。
2. 輸入儲存庫名稱（例如 `tcm-tracker`），設定為 **Public**，點擊 **Create repository**。
3. 點擊 **uploading an existing file**，將本壓縮包解壓後的全部檔案拖曳上傳，點擊 **Commit changes**。
4. 進入該 Repository 的 **Settings** -> 左側選單點擊 **Pages**。
5. 在 **Build and deployment** 下的 **Branch** 選擇 `main`（或 `master`）及 `/(root)`，點擊 **Save**。
6. 等待約 1–2 分鐘，頁面頂部即會顯示你的專屬 HTTPS 網址：`https://<你的帳號>.github.io/tcm-tracker/`。

## 📲 手機瀏覽器安裝與離線使用說明

- **Android (Chrome / Edge)**：以 Chrome 開啟上述 HTTPS 網址，等待 2 秒讓頁面頂部顯示「● 離線安裝就緒 (PWA)」，點擊頂部「📲 安裝應用」按鈕（或瀏覽器右上角選單 `⋮` -> **安裝應用程式 / 加到主畫面**）。
- **iPhone / iPad (Safari)**：以 Safari 開啟上述 HTTPS 網址，點擊底部中間的「分享」圖示 -> 選擇 **「加入主畫面」**。
- **離線使用提示**：首次在瀏覽器點選「📷 拍照」時請選擇「允許使用攝像頭」；建議定期於「💾 備份與管理」點擊「⬇️ 匯出 JSON 完整備份」將資料備份至手機檔案夾，以防清除瀏覽器快取時遺失資料。
