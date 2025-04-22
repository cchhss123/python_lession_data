## [單元 4：Python 資料處理與分析]

**簡介：** 本單元將深入學習使用 Pandas 和 NumPy 進行資料的載入、檢視、清理、轉換、篩選、排序、分組聚合等核心操作，並介紹使用 Matplotlib 和 Seaborn 進行資料視覺化。

### 3.1 Pandas 基礎

  * **DataFrame 和 Series 物件：**
      * 創建 DataFrame 和 Series
      * 從不同資料來源創建 DataFrame
      * DataFrame 的基本屬性 (shape, index, columns, dtypes)
      * Series 的基本屬性 (index, values, dtype)
  * **資料的載入與儲存：**
      * 載入不同格式的資料 (`read_csv`, `read_excel`, `read_json` 等)
      * 儲存資料 (`to_csv`, `to_excel`, `to_json` 等)
  * **資料的檢視：**
      * `head()`, `tail()`
      * `info()`
      * `describe()`
      * `value_counts()`

### 3.2 資料清理

  * **處理遺失值 (Missing Values)：**
      * 識別遺失值 (`isnull()`, `notnull()`)
      * 處理遺失值的方法 (`dropna()`, `fillna()`)
      * 插值填補 (`interpolate()`)
  * **處理重複值 (Duplicates)：**
      * 識別重複值 (`duplicated()`)
      * 移除重複值 (`drop_duplicates()`)
  * **資料類型轉換 (Data Type Conversion)：**
      * 使用 `astype()` 轉換資料類型
      * 處理日期時間資料 (`to_datetime()`)
      * 轉換數值和類別資料

### 3.3 資料轉換

  * **新增和刪除欄位：**
      * 直接賦值新增欄位
      * 使用 `insert()` 在指定位置新增欄位
      * 使用 `drop()` 刪除欄位
  * **資料的篩選 (Filtering)：**
      * 使用布林索引進行篩選
      * 使用 `loc[]` 和 `iloc[]` 進行選擇
      * 使用條件表達式進行篩選
  * **資料的排序 (Sorting)：**
      * 按索引排序 (`sort_index()`)
      * 按值排序 (`sort_values()`)
  * **資料的分組聚合 (Grouping and Aggregation)：**
      * 使用 `groupby()` 進行分組
      * 常用的聚合函數 (`mean()`, `sum()`, `count()`, `min()`, `max()`, `std()` 等)
      * 應用多個聚合函數 (`agg()`)
      * 轉換和過濾分組 (`transform()`, `filter()`)
  * **資料的合併 (Merging) 和連接 (Concatenating)：**
      * 使用 `merge()` 合併 DataFrame (類似 SQL JOIN)
      * 使用 `concat()` 連接 DataFrame

### 3.4 資料探索性分析 (Exploratory Data Analysis - EDA) 與視覺化

  * **使用 Matplotlib 進行基本繪圖：**
      * 折線圖 (`plot()`)
      * 散佈圖 (`scatter()`)
      * 長條圖 (`bar()`, `barh()`)
      * 直方圖 (`hist()`)
      * 盒鬚圖 (`boxplot()`)
      * 餅圖 (`pie()`)
      * 子圖 (`subplot()`)
      * 自訂圖表的標題、標籤、圖例等
  * **使用 Seaborn 進行更進階的統計圖形繪製：**
      * 分布圖 (`histplot()`, `kdeplot()`, `displot()`)
      * 關係圖 (`scatterplot()`, `lineplot()`, `pairplot()`)
      * 類別圖 (`boxplot()`, `violinplot()`, `barplot()`, `countplot()`)
      * 熱力圖 (`heatmap()`)
      * 風格和調色板的設定

**實作練習：**

  * 載入一個 OpenData 資料集。
  * 檢視資料的基本資訊和統計摘要。
  * 處理資料中的遺失值或重複值。
  * 根據特定條件篩選資料。
  * 對資料進行分組並計算聚合統計量。
  * 使用 Matplotlib 和 Seaborn 繪製至少三種不同的圖表來探索資料的特性。