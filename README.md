# 📊 Trader Performance & Market Sentiment Analysis

## 📝 Project Overview
This project explores the **relationship between trader performance and market sentiment** (Fear vs. Greed regimes).  
The goal is to **uncover hidden behavioral patterns, risks, and predictive signals** that can inform smarter trading strategies.

The analysis leverages:
- Exploratory Data Analysis (EDA) & Time Series Trends
- Behavioral Analytics of traders during different sentiment regimes
- Machine Learning Models (XGBoost, LightGBM) with SHAP explainability
- Risk & Anomaly Detection (identifying overtrading/risk clusters)
- Portfolio Strategy Backtesting (Sentiment vs. Volatility signals)

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/tatseek/DS_Arunima_Das.git
cd DS_Arunima_Das
```
### 2. Create Virtual Environment
```bash
python3 -m venv venv
source venv/bin/activate   # for Linux/Mac
venv\Scripts\activate      # for Windows
```
### 3. Data Preparation 
```
- Place the required CSV datasets in the csv_file.
- Ensure the structure matches the inputs expected by notebook_1.ipynb and notebook_2.ipynb.

Example dataset fields:
timestamp, account, pnl, sentiment_score, trade_count, volatility, size_usd, fee, side
```
### 4. Running the analysis
```
1. jupyter lab
- if opening from jupyter lab ,
  #from google.colab import drive
  #drive.mount('/content/drive')
- Ammend correct paths to each file as per your folder location .

2. Google colab
- run the codes directly , (after ammending the corrct paths to each files)

ORDER OF RUNNING BOTH FILES
--notebook_1.ipynb → Exploratory analysis, sentiment impact, behavioral patterns, baseline ML.
-- notebook_2.ipynb → Advanced ML models, anomaly detection, portfolio optimization.
```
### 5. Project Structure
```
DS_Arunima_Das/
├── notebook_1.ipynb          # EDA, Time Series, Behavioral Analytics
|── notebook_2.ipynb          # Advanced ML, Risk Analysis, Portfolio Strategies
├── csv_file                  # Store all csv 
    └──fear_greed_index.csv   #Contains Sentiment Dataset
    └──historical_data.csv    #Contains historical trade data from hyperliquid
├── output/                   #Stores all visual outputs, graphs and charts and csv output too
├── DS_report.pdf/            # Final reports including explanation 
└── README.md                 # Project documentation including setup, instructions and notes
```


