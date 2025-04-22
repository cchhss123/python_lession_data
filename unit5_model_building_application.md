## [單元 5：模型建立與應用]

**簡介：** 本單元將簡要介紹機器學習的基本概念與流程，並學習使用 Scikit-learn 建立和評估簡單的監督式學習模型，最後示範如何將模型應用於實際問題。

### 4.1 機器學習基礎概念

  * 什麼是機器學習？與資料分析的關係
  * 監督式學習、非監督式學習、強化學習簡介
  * 監督式學習的基本流程：
      * 資料準備 (特徵工程、資料分割)
      * 模型選擇
      * 模型訓練
      * 模型評估
      * 模型部署與應用
  * 常見的機器學習任務：
      * 分類 (Classification)
      * 回歸 (Regression)

### 4.2 使用 Scikit-learn 建立監督式學習模型

  * **資料準備：**
      * 特徵 (Features) 和目標變數 (Target Variable) 的概念
      * 將資料分割為訓練集和測試集 (`train_test_split()`)
      * 簡單的特徵工程 (例如：處理類別變數 - One-Hot Encoding)
      * 特徵縮放 (`StandardScaler`, `MinMaxScaler`) 的基本概念
  * **分類模型：**
      * 線性模型：邏輯回歸 (`LogisticRegression`)
      * 樹模型：決策樹 (`DecisionTreeClassifier`)、隨機森林 (`RandomForestClassifier`)
      * 模型訓練 (`fit()`)
      * 模型預測 (`predict()`, `predict_proba()`)
  * **回歸模型：**
      * 線性模型：線性回歸 (`LinearRegression`)
      * 樹模型：決策樹回歸 (`DecisionTreeRegressor`)、隨機森林回歸 (`RandomForestRegressor`)
      * 模型訓練 (`fit()`)
      * 模型預測 (`predict()`)

### 4.3 模型評估

  * **分類模型評估指標：**
      * 準確率 (Accuracy)
      * 精確度 (Precision)、召回率 (Recall)、F1 分數
      * 混淆矩陣 (Confusion Matrix)
      * AUC-ROC 曲線
      * 使用 Scikit-learn 的評估函數 (`accuracy_score()`, `precision_score()`, `recall_score()`, `f1_score()`, `confusion_matrix()`, `roc_auc_score()`, `roc_curve()`)
  * **回歸模型評估指標：**
      * 均方誤差 (Mean Squared Error - MSE)
      * 均方根誤差 (Root Mean Squared Error - RMSE)
      * 平均絕對誤差 (Mean Absolute Error - MAE)
      * R 平方 (R-squared)
      * 使用 Scikit-learn 的評估函數 (`mean_squared_error()`, `mean_absolute_error()`, `r2_score()`)

### 4.4 模型應用

  * 將訓練好的模型應用於新的資料進行預測
  * 模型持久化 (儲存和載入模型 - `pickle`, `joblib`)
  * 簡單的模型部署概念 (例如：將模型整合到一個簡單的應用程式中)

**實作練習：**

  * 選擇一個適合的 OpenData 資料集進行分類或回歸任務。
  * 使用 Pandas 載入並準備資料。
  * 將資料分割為訓練集和測試集。
  * 訓練一個或多個 Scikit-learn 模型。
  * 使用適當的評估指標評估模型的性能。
  * 使用訓練好的模型對測試集中的資料進行預測。