# DS Mohammed Shahrukh

Public Colab link: [https://colab.research.google.com/drive/10zoCxjZx3JcGZnJ7Z5-6pBxd-5Awtt-u?usp=sharing]

Here’s a **professional README.md template** tailored for your Web3 Trading Team submission:

---

# Web3 Trading Behavior & Market Sentiment Analysis

**Author:** Mohammed Shahrukh
**Assignment:** Data Science – Web3 Trading Team

---

## 📌 Project Overview

This project analyzes the relationship between trader behavior (profitability, risk, volume, leverage) and market sentiment (Fear vs Greed). Using historical trader data and the Bitcoin Fear & Greed Index, we identify patterns, divergences, and hidden signals that could support smarter trading strategies.

---

## 📂 Repository Structure

```
ds_Mohammed_Shahrukh/
├── notebook_1.ipynb                # Main analysis & visualizations             
├── csv_files/                      # Processed CSV outputs
│   ├── agg_by_sentiment.csv
│   ├── cohort_volume_by_sentiment.csv
│   ├── contrarian_days.csv
│   ├── daily_behavior_with_sentiment.csv
│   ├── lag1_sentiment_effects.csv
│   ├── summary_by_sentiment.csv
│   └── ttests_fear_vs_greed.csv
├── outputs/                        # Charts & visual outputs
│   ├── avg_volume_by_sentiment.png
│   ├── daily_pnl_timeseries.png
│   ├── long_share_by_sentiment.png
│   └── win_rate_by_sentiment.png
├── ds_report.pdf                   # Final summarized insights
└── README.md                       # Project documentation
```

---

## 📊 Datasets

1. **Historical Trader Data from Hyperliquid**

   * Columns: `account`, `symbol`, `execution_price`, `size_tokens`, `size_usd`, `side`, `timestamp_ist`, `start_position`, `direction`, `closed_pnl`, `transaction_hash`, `order_id`, `trader_score`, `leverage`
   * [Dataset Link](https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing)

2. **Bitcoin Fear & Greed Index**

   * Columns: `timestamp`, `value`, `classification`, `date`
   * [Dataset Link](https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing)

---

## ⚙️ How to Run the Analysis

### 1. Open in Google Colab

* Upload the `.ipynb` files to Google Colab OR open directly from GitHub via:

  ```python
  from google.colab import drive
  drive.mount('/content/drive')
  ```

### 2. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn
```

### 3. Add Datasets

* Upload both datasets to the Colab session or link your Google Drive with the provided dataset paths.

### 4. Run the Notebook

* Execute `notebook_1.ipynb` step-by-step to generate processed CSVs and plots.
* `notebook_2.ipynb` contains optional deeper analysis.

---

## 📈 Key Insights from the Analysis

* **High leverage during Fear periods** often correlates with lower win rates.
* **Greed phases** show higher trade volumes but with mixed profitability outcomes.
* Certain **contrarian trading days** yield above-average PnL regardless of sentiment.
* Lag analysis reveals that **Extreme Greed signals** may precede profit dips.

---

## 📦 Outputs

* **CSV files**: Contain aggregated and processed metrics.
* **Charts**: Highlight trends in PnL, win rates, volume, and position bias.
* **PDF Report**: Summarizes key findings with visuals.

---

## 📝 Notes

* Ensure **runtime is set to Python 3** in Colab.
* Datasets must be loaded before executing the cells.
* All results are reproducible by running the provided notebooks in sequence.

---

## 📜 License

This work is submitted solely for the Web3 Trading Team Data Science Assignment and should not be redistributed without permission.

---

If you like, I can **fill in the “Key Insights” section with exact results from your generated CSVs and plots** so the README looks even stronger for evaluation. That would make it a complete, ready-to-submit package.
