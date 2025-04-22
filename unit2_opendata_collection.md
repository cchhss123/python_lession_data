## [單元 2：OpenData 資料蒐集]

**簡介：** 本單元將介紹 OpenData 的概念與常見平台，並學習如何使用 Python 從網路或檔案系統中獲取不同格式的 OpenData。

### 2.1 什麼是 OpenData？

  * 定義與重要性
  * OpenData 的原則與許可協議
  * 常見的 OpenData 平台介紹：
      * 政府開放資料平台（台灣、國際）
      * 學術機構、研究單位發布的資料
      * 企業或組織公開的資料
      * API 形式的 OpenData

### 2.2 使用 Python 進行網路資料蒐集

  * **使用 `requests` 函式庫：**
      * 發送 HTTP 請求 (GET, POST)
      * 處理回應 (狀態碼、標頭、內容)
      * 下載檔案
      * 簡單的網頁爬蟲概念 (robots.txt 注意事項)
  * **使用 `urllib` 函式庫：**
      * 基本 URL 操作
      * 開啟和讀取網路資源

### 2.3 處理常見的 OpenData 格式

  * **CSV (Comma Separated Values)：**
      * 使用 Pandas 的 `read_csv()` 讀取 CSV 檔案
      * 處理不同的分隔符、編碼格式
      * 從網路 URL 讀取 CSV
  * **JSON (JavaScript Object Notation)：**
      * 使用 Python 的 `json` 函式庫解析 JSON 資料
      * 使用 Pandas 的 `read_json()` 讀取 JSON 檔案
      * 處理巢狀 JSON 資料
      * 從 API 獲取 JSON 資料
  * **XML (Extensible Markup Language)：**
      * 使用 `xml.etree.ElementTree` 或 `lxml` 函式庫解析 XML 資料
      * 提取 XML 元素和屬性
      * 將 XML 資料轉換為 Pandas DataFrame
  * **其他常見格式簡介 (例如：Excel, GeoJSON 等)**

### 2.4 OpenData API 的使用

  * 什麼是 API (Application Programming Interface)
  * 常見的 API 類型 (RESTful API)
  * 使用 `requests` 函式庫與 API 互動
  * 處理 API 回應 (JSON 格式為主)
  * API 身份驗證 (API Keys, OAuth 等)
  * API 請求的限制與最佳實踐

**實作練習：**

  * 從政府開放資料平台下載一個 CSV 或 JSON 檔案。
  * 使用 Pandas 讀取下載的檔案並顯示前幾行。
  * 使用 `requests` 函式庫獲取一個簡單的網路頁面的內容。
  * 嘗試使用一個公開的 API 獲取資料（例如：天氣 API）。