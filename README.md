# Trader Performance vs Market Sentiment Analysis
---

## Notebook Descriptions

### Notebook 1 — Data Pipeline & Exploratory Analysis
Covers:
- Environment setup and project structure
- Trade data ingestion and validation
- Market sentiment encoding (binary and ordinal)
- Leakage-safe sentiment alignment
- Feature engineering (profitability, risk, behavior)
- Exploratory data analysis across sentiment regimes

**Output:**  
A feature-complete dataset (`trades_features.csv`) and core exploratory insights.


### Notebook 2 — Behavioral & Strategy Analysis
Extends the analysis by focusing on:
- Contrarian vs momentum strategy performance
- Trader archetype identification using clustering
- Risk dynamics during extreme fear and extreme greed
- Tail-risk and exposure escalation analysis
- Robustness checks using outlier trimming
---

## Dataset Description

### 1. Historical Trader Data (historical_data.csv)
Contains detailed trade-level information. 

Each row represents a completed trade.

### 2. Bitcoin Fear & Greed Index (fear_greed_index.csv)
Provides daily market sentiment labels.

This dataset captures market psychology rather than price movements.
---

## Tools & Libraries
- Python (Jupyter Notebook)
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
---

## How to Run
1. Clone the repository
   
 ```bash
git clone https://github.com/DeadBoTt-exe/Assignment_Primetrade.ai.git
```

2. Install dependencies
   
 ```bash
pip install -r requirements.txt
```

4. Run `notebook1.ipynb` first to generate feature datasets
5. Run `notebook2.ipynb` for advanced analysis and insights
---

## Project Structure

```
Assignment_Primetrade.ai
|
├── csv_files/
│   ├── historical_data.csv
│   ├── fear_greed_index.csv
│   ├── trades_with_sentiment.csv
│   └── trades_features.csv
│
├── outputs/
│   ├── trade_count_by_sentiment.png
│   ├── avg_pnl_by_sentiment.png
│   ├── ....
│   ├── ....
│   ├── tail_loss_extreme_sentiment.png
│   └── robustness_strategy_comparison.png
│
├── .gitignore
├── notebook1.ipynb
├── notebook2.ipynb
├── ds_report.pdf
└── README.md

```
