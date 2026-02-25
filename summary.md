# 2026-02-25 開發紀錄

![網站預覽](./screenshot.png)

## 專案：Meng 個人網站 (DeepRL-DIC1)

今天主要完成了 Meng 的單頁式個人網站開發，以及將專案部署到 GitHub 上。以下是詳細的開發紀錄：

### 1. 介面設計與開發 (UI/UX)
*   **深色模式 (Dark Theme)**：採用現代化的深色背景，搭配微光澤的磨砂玻璃 (Glassmorphism) 效果，營造出科技感與質感。
*   **動態排版**：
    *   **置中佈局**：使用 Flexbox 和 Grid 使畫面元素在不同裝置上都能完美置中。
    *   **響應式設計 (RWD)**：確保在手機、平板與桌機上都有良好的瀏覽體驗。
*   **視覺元素**：
    *   **大頭貼**：加入了圓形遮罩與漸層光環，配合呼吸燈動畫 `pulse`。
    *   **標題與介紹**：設計了醒目的 "Hello, I'm Meng" 標題，搭配下方精簡的個人介紹。
    *   **社群圖示**：使用 FontAwesome 圖示連結至 GitHub 等社群平台，具有懸停 (Hover) 時的放大與發光效果。

### 2. 即時時鐘功能 (JavaScript)
*   **動態時間顯示**：使用 JavaScript 的 `Date` 物件與 `setInterval` 函數，實作了每秒更新的數位時鐘。
*   **時間格式化**：確保時間的時、分、秒都是兩位數顯示（例如：09:05:03）。
*   **日期顯示**：除時間外，也加上了目前的年月日星期顯示。

### 3. Git 與 GitHub 部署
完成程式碼後，將本機的專案推送到指定的 GitHub 資料庫 (https://github.com/mengbei0116/DeepRL-DIC1)：
*   初始化 Git：`git init` 及 `git add .`。
*   設定 Git 使用者名稱與信箱：`mengbei0116` / `mengbei0116@users.noreply.github.com`。
*   進行初始的 Commit：`git commit -m "Initial commit"`。
*   切換主分支為 `main`：`git branch -M main`。
*   連結遠端資料庫並推送程式碼：`git remote add origin ...` 及 `git push -u origin main`。

### 4. 後續建議設定
*   **GitHub Pages**：可以前往 GitHub 資料庫的 Settings -> Pages，將來源 (Source) 設定為 `main` 分支的 `/ (root)`，即可獲得一個免費的專屬網址，讓其他人能直接在網路上看到這個作品。
