每日單字 PWA 免費版

內容：
- 單字新增、搜尋、編輯、刪除
- 中文遮蔽與單字發音查詢（開啟 Cambridge Dictionary）
- 本機自動儲存
- 已熟悉標記、隨機選擇題
- JSON 備份、CSV 匯出、JSON/CSV 匯入
- PWA 可安裝及離線快取

重要限制：
1. 單字存在當前瀏覽器本機，不是雲端同步。請定期匯出備份。
2. 快速例句為模板產生，不是 AI。真正 AI 生成需另接服務/API。
3. Cambridge 發音按鈕會開啟字典網頁，非將音訊嵌入應用。
4. PWA 必須經 HTTPS 或 localhost 提供，直接雙擊 index.html 時安裝/離線功能可能不可用。

部署（免費）：
A. GitHub Pages
1. 登入 GitHub，建立公開 repository（例如 vocab-app）。
2. 將此 ZIP 解壓，將 index.html、manifest.json、sw.js、icon.svg 上傳到 repository 根目錄。
3. Repository → Settings → Pages → Deploy from a branch → main / root → Save。
4. 等待 Pages 顯示網址，使用該 HTTPS 網址開啟。

B. 本機測試
若電腦有 Python，在此資料夾開終端機執行：
python -m http.server 8000
瀏覽 http://localhost:8000

安裝：
- Android Chrome：開啟已部署 HTTPS 網址 → 瀏覽器選單 → 安裝應用程式／加入主畫面。
- iPhone Safari：分享 → 加入主畫面。
- 電腦 Chrome/Edge：網址列附近若顯示安裝圖示，點選安裝；或瀏覽器選單中找「安裝頁面為應用程式」。

CSV 欄位：
English,Chinese,Example,Translation,Level
