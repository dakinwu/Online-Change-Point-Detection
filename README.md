# Online-Change-Point-Detection (OCPD)  
線上轉折點偵測（OCPD）

## 專案簡介 | Project Overview

本專案旨在將多變量線上轉折點偵測（OCPD）方法延伸至函數型資料（Functional Data），以即時且有效地偵測資料流中的異常變化。透過模擬實驗，評估各種方法在平均運行長度（Average Run Length, ARL）與平均檢測延遲（Average Detection Delay, ADD）兩大指標下的表現，並探討其在不同變異類型（均值、變異數、共變異數等）下的偵測能力與改進潛力。

This project aims to extend multivariate online changepoint detection (OCPD) methods to functional data, enabling real-time and effective detection of anomalies in data streams. Through simulation experiments, we evaluate the performance of various methods using two key metrics: Average Run Length (ARL) and Average Detection Delay (ADD). We further investigate detection capabilities under different types of changes (mean, variance, covariance, etc.) and explore potential improvements.

---

## 方法與流程 | Methods & Workflow

- **資料模擬**：產生不同型態的函數型資料流，包含均值變化、變異數變化、共變異數變化及無變化等情境。
- **OCPD 方法實作**：實現多種線上轉折點偵測方法，並針對函數型資料特性進行調整與優化。
- **效能評估**：以 ARL 與 ADD 為主要指標，系統性比較各方法於不同變化類型下的偵測效能。
- **結果分析**：彙整模擬結果，探討各方法優缺點及未來改進方向。

- **Data Simulation**: Generate functional data streams with various change scenarios, including mean shifts, variance changes, covariance changes, and no change.
- **OCPD Implementation**: Implement multiple online changepoint detection methods, adapting and optimizing them for functional data characteristics.
- **Performance Evaluation**: Systematically compare detection performance using ARL and ADD as primary metrics across different change types.
- **Result Analysis**: Summarize simulation outcomes, discuss strengths and weaknesses of each method, and propose directions for future improvement.

---

## 資料結構 | Data Structure

- `cc_rho0.2/`, `gstream_deriv_rho0.2/`, `gstream_eucli_rho0.2/`, `real_rho0.2/`, `energy/`  
  儲存各種模擬情境下的 RDS 結果檔案，涵蓋不同變化類型與參數設定。
- `.Rmd` 檔案  
  包含分析流程、圖表繪製與結果彙整的 R Markdown 文件。
- `gstream.R`  
  主要演算法與資料處理程式碼。

- `cc_rho0.2/`, `gstream_deriv_rho0.2/`, `gstream_eucli_rho0.2/`, `real_rho0.2/`, `energy/`  
  Store RDS result files for various simulation scenarios, covering different change types and parameter settings.
- `.Rmd` files  
  R Markdown documents for analysis workflow, visualization, and result summary.
- `gstream.R`  
  Main algorithm and data processing scripts.

---

## 評估指標 | Evaluation Metrics

- **平均運行長度（ARL）**：在無變化情境下，方法發生誤報前的平均觀測次數。
- **平均檢測延遲（ADD）**：在變化發生後，方法成功偵測所需的平均延遲時間。

- **Average Run Length (ARL)**: The average number of observations before a false alarm occurs under no-change scenarios.
- **Average Detection Delay (ADD)**: The average delay required to successfully detect a change after it occurs.

---

## 專案貢獻 | Contributions

- 提供一套完整的函數型資料線上轉折點偵測評估框架。
- 系統性比較多種 OCPD 方法於不同變化類型下的效能。
- 為未來函數型資料異常偵測方法的開發與應用提供參考依據。

- Provides a comprehensive evaluation framework for online changepoint detection in functional data.
- Systematically compares the performance of various OCPD methods under different change scenarios.
- Offers valuable references for future development and application of anomaly detection methods in functional data analysis.

---

## 聯絡方式 | Contact

如有任何問題或合作意願，歡迎聯絡專案負責人。  
For questions or collaboration, please contact the project maintainer.
