# Node.js AWS S3 Integration Project

## 簡介
這個專案是一個基於 Node.js 的 AWS Lambda 函數，旨在從一個指定的 URL 獲取調查數據，並將相應的信息更新到 AWS S3 中的 JSON 檔案。該函數用於特定的數據處理任務，透過解析 HTTP 請求的主體來提取必要的參數，然後進行操作。

## 功能
- 從 HTTP 請求中解析 SVID 及 HASH 參數。
- 根據提取的參數向指定的 URL 發送請求以獲取調查數據。
- 根據調查數據更新 S3 中特定 JSON 檔案的內容。
- 定期讀取 S3 中的 JSON 資料。

## 安裝與使用方式
1. 確保你的環境中已安裝 Node.js 和 NPM。
2. 克隆這個專案到本地：
   ```bash
   git clone https://github.com/your-username/aws-s3-integration.git
   cd aws-s3-integration
   ```
3. 安裝必要的依賴：
   ```bash
   npm install aws-sdk node-fetch
   ```
4. 在程式碼中填入你的 AWS 訪問金鑰及相關設定。
5. 部署該 Lambda 函數至 AWS，並根據需求設置觸發條件。

## 必要的依賴模組清單
- `aws-sdk`：AWS SDK for JavaScript，用於操作 AWS 服務。
- `node-fetch`：用於發送 HTTP 請求的輕量級模組。

## 授權條款
本專案基於 MIT 證書授權，詳情請參閱 [LICENSE](LICENSE) 檔案。