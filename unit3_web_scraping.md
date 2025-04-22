## [單元 3：網路爬蟲與網站資料擷取]

**簡介：** 本單元將專門介紹網路爬蟲的概念、道德與法律考量，並深入學習使用 Python 函式庫來擷取網站上的資料。

### 3.1 網路爬蟲基礎

  * **什麼是網路爬蟲 (Web Crawler / Spider)？**
      * 工作原理：發送請求、接收回應、解析內容、提取資料、追蹤連結
      * 常見應用場景
  * **網路爬蟲的類型**
      * 通用爬蟲 (General-purpose Web Crawler)
      * 定向爬蟲 (Focused Crawler / Topical Crawler)
      * 增量式爬蟲 (Incremental Crawler)
  * **網路請求與回應**
      * HTTP 協議 (GET, POST 等)
      * HTTP 狀態碼
      * Request Headers 和 Response Headers
  * **網頁結構基礎**
      * HTML (HyperText Markup Language)
      * CSS (Cascading Style Sheets)
      * JavaScript

### 3.2 道德與法律考量

  * **`robots.txt` 協議**
      * 了解和遵守 `robots.txt` 的規則
      * 常見的 Disallow 和 Allow 指令
  * **網站的使用條款 (Terms of Service)**
      * 仔細閱讀並遵守網站的爬取政策
  * **避免對網站造成過度負載**
      * 設定合理的請求間隔 (delay)
      * 限制並發請求的數量
  * **資料隱私與版權問題**
      * 尊重個人隱私
      * 避免侵犯網站內容的版權
  * **法律風險**
      * 了解相關法律法規

### 3.3 Python 爬蟲常用函式庫

  * **`requests`：** 發送 HTTP 請求，獲取網頁內容。
      * 發送不同類型的請求
      * 處理 Cookies 和 Sessions
      * 設定代理 IP
      * 處理逾時和錯誤
  * **`Beautiful Soup` (`bs4`)：** 解析 HTML 和 XML 文件。
      * BeautifulSoup 物件的創建
      * 導航樹狀結構 (Tag, NavigableString, BeautifulSoup 物件)
      * 搜尋元素：
          * `find()` 和 `find_all()`
          * 使用標籤名、屬性、文字內容進行搜尋
          * CSS 選擇器 (`select()`)
  * **`lxml`：** 更快速和強大的 XML 和 HTML 解析器。
      * 安裝和使用 `lxml`
      * XPath 語法入門
      * 使用 XPath 提取資料
  * **`Scrapy`：** 強大的網路爬蟲框架。
      * Scrapy 的架構 (Spiders, Items, Pipelines, Middlewares 等)
      * 創建 Scrapy 專案和 Spider
      * 定義 Items 來儲存爬取到的資料
      * 使用 Selectors (基於 CSS 和 XPath) 提取資料
      * 使用 Pipelines 處理和儲存資料
      * 處理翻頁、登入、表單提交等常見爬蟲任務
      * Scrapy 的優勢和適用場景
  * **處理動態網頁內容**
      * `Selenium`：模擬瀏覽器行為，可以執行 JavaScript。
          * WebDriver 的基本操作 (開啟網頁、查找元素、點擊、輸入等)
          * 處理彈出視窗、Alerts 等
      * `Playwright`：由 Microsoft 開發的現代化端對端測試框架，也可用於網頁爬取。
          * 類似 Selenium 的功能，但通常更快速和穩定。
      * API 渲染服務 (例如：`scrapy-splash`)

### 3.4 實戰案例

  * 爬取特定網站的新聞標題和連結
  * 爬取電商網站的商品資訊（名稱、價格、圖片連結）
  * 爬取股票資訊或匯率資料
  * 處理需要登入的網站
  * 處理翻頁和分頁
  * 簡單的反爬蟲策略與應對（User-Agent 偽裝、請求延遲等）

### 3.5 資料儲存

  * 將爬取到的資料儲存為 CSV、JSON 等檔案
  * 儲存到資料庫 (例如：SQLite, MySQL, PostgreSQL, MongoDB)

**實作練習：**

  * 使用 `requests` 和 `Beautiful Soup` 爬取一個簡單的靜態網頁，提取特定資訊。
  * 練習使用 CSS 選擇器和 XPath 語法定位網頁元素。
  * 嘗試使用 `Scrapy` 建立一個簡單的爬蟲專案。
