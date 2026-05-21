# 產品碳足跡計算助理
## Product Carbon Footprint Assistant

> 基於 U.S. EPA USEEIO Supply Chain GHG Emission Factors v1.3.0 的支出基礎環境投入產出（Spend-based EEIO）碳足跡估算工具

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-Try_Now-success.svg)](https://carbon-footprint-johnny.netlify.app)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Methodology](https://img.shields.io/badge/Methodology-Spend--based%20EEIO-green.svg)]()
[![Base Year](https://img.shields.io/badge/Base%20Year-USD%202022-blue.svg)]()

---

## 工具特色 · Features

- ✅ **完整涵蓋 1,016 個 NAICS-6 產業類別**（U.S. EPA 官方分類）
- ✅ **中英雙語介面**,支援 813+ 條中文對照詞、59 個歧義詞智能消歧
- ✅ **採購方／販售方雙視角**自動切換含加成（with margins）／不含加成（without margins）係數
- ✅ **2022 年均匯率基準**（1 USD = 29.782 TWD），與排放係數計價年一致
- ✅ **純前端純隱私**:所有計算在瀏覽器執行,採購金額與產品名稱**不傳到任何伺服器**
- ✅ **透明計算鏈**:每筆估算顯示完整 NAICS 對應、係數來源、換算邏輯

## 適用情境 · Use Cases

| 適合 | 不適合 |
|---|---|
| ✅ 組織採購碳盤查熱點辨識 | ❌ 單一產品對外碳標籤宣稱 |
| ✅ ESG 範疇三快速估算 | ❌ ISO 14067 製程生命週期分析(LCA)|
| ✅ 供應商篩選與排序 | ❌ 取代第三方查證之精確盤查 |
| ✅ 碳管理教育與顧問實務 | ❌ 法規申報主要依據 |

## 方法論 · Methodology

本工具採**支出基礎環境投入產出法(Spend-based Environmentally-Extended Input-Output, EEIO)**,計算公式:

碳足跡(kg CO₂e) = 採購金額(TWD) ÷ 匯率(TWD/USD) × 排放係數(kg CO₂e/USD)

**資料來源**:
- 排放係數:[U.S. EPA Supply Chain GHG Emission Factors v1.3.0](https://www.epa.gov/climateleadership/supply-chain-greenhouse-gas-emission-factors)
- 產業分類:[NAICS 2017](https://www.census.gov/naics/)
- 貨幣基準:2022 USD, purchaser price

## 不確定性聲明 · Uncertainty Disclaimer

【方法論】NAICS 為產業分類,同類別下不同產品共用同一係數,無法區分個別產品差異。本工具結果為「該產業類別平均」的供應鏈碳排估計值,非特定產品的精確實測值。

【建議查證】跨系統引用同一 NAICS 可能因下列原因產生差異,比對前請確認:
- 不同模型版本(v1.0–v1.3 之間係數會微調)
- 不同貨幣基準年(USD2017/2020/2021/2022)
- 不同氣體口徑(All GHGs vs 僅 CO₂)
- 對應到不同 NAICS 代碼

## 使用方式 · Usage

### 線上使用(推薦)
🚀 **[立即開啟工具 · Launch Tool](https://carbon-footprint-johnny.netlify.app)**

直接造訪上方連結即可使用,無需安裝任何軟體。

### 本機使用
1. 下載 `index.html`
2. 雙擊以瀏覽器打開
3. 即可離線使用

## 版本歷史 · Version History

| 版本 | 日期 | 主要更新 |
|---|---|---|
| v1.0 | 2026-05-20 | 初始版本:1,016 NAICS 類別、813 中文對照詞、59 歧義詞 |

## 引用方式 · Citation

若您在學術或專業報告中使用本工具,建議引用如下:
陳懷傑(Johnny Chen). (2026). 產品碳足跡計算助理 [Product Carbon Footprint Assistant]
(Version 1.0) [Software]. GitHub.
https://github.com/johnnyweb-art/carbon-footprint-tool

## 授權 · License

本專案採 [MIT License](LICENSE) 授權。歡迎自由使用、修改、再散布,但須保留原作者著作權聲明。

排放係數資料屬美國環境保護署(U.S. EPA)公開資料,依其使用條款使用。

## 開發者 · Developer

**陳懷傑(Johnny Chen)**
- 元智大學管理學院助理教授
- 校級創新創業中心主任
- 管理學院就業暨校友服務中心主任
- 研究領域:人力資源管理、組織行為、ESG 永續治理、創新創業教育

## 致謝 · Acknowledgments

- U.S. EPA 提供開放的供應鏈溫室氣體排放係數資料
- NAICS 美國北美產業分類系統作為產業歸類基礎
- MOEA 中小企業營運升級顧問計畫、TTQS 訓練品質評核、USR 計畫實務應用啟發

---

**最後更新 Last Updated**:2026-05-20
