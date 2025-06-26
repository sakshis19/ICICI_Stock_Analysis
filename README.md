# 📈 ICICI Bank Stock Market Data Analysis using PySpark
---

## 📝 Overview

This project aims to analyze historical stock market data for **ICICI Bank** using **Apache Spark (PySpark)**. We perform comprehensive data cleaning, exploratory data analysis (EDA), correlation analysis, and trend discovery to extract actionable insights for traders, investors, and analysts. The analysis is entirely built on distributed computing principles using PySpark.

---

## 🗂️ Project Workflow

### ✅ Phase 1: Setup & Data Exploration
- Load the `ICICIBANK.csv` dataset using Spark.
- Understand data structure using `.show()`, `.printSchema()`, `.describe()`.
- Register DataFrame as a temporary SQL view for basic queries.

### ✅ Phase 2: Data Cleaning & Feature Engineering
- Handle missing values and drop duplicates.
- Convert date columns to `DateType`.
- Add key columns:
  - **Daily Returns** (day-over-day percentage change)
  - **50-day & 200-day Simple Moving Averages (SMA)**

### ✅ Phase 3: Exploratory Data Analysis
- Analyze Open, Close, Volume, and Returns.
- Examine:
  - Volatility using standard deviation
  - Seasonal patterns by month
  - Trends using SMA crossovers
  - Periods of high/low trading volume

### ✅ Phase 4: Correlation & Trend Analysis
- Calculate correlation between Volume and Price.
- Identify significant moving average crossovers (Buy/Sell signals).
- Analyze outliers in returns related to market events.

### ✅ Phase 5: Strategic Insights
- Provide investor-friendly summaries based on:
  - Volatility trends
  - Seasonal patterns
  - Volume-price dynamics
  - SMA crossovers

---

## 💡 Key Findings

| Metric                 | Insight                                                                 |
|------------------------|-------------------------------------------------------------------------|
| 📊 Price Trends        | SMA crossovers indicate bullish/bearish momentum shifts                 |
| 📈 Volatility          | High volatility aligns with news-driven market events                  |
| 🔄 Volume Correlation  | Moderate correlation with closing price movement                        |
| 📅 Seasonality         | Monthly trends reveal consistent up/down periods for strategic entries  |
| ⚠️ Outliers            | Spikes in returns often follow major financial announcements            |

---

## 📌 How to Run This Project

1. **Clone the Repository**
   ```bash
   git clone https://github.com/sakshis19/ICICI-Bank-Stock-Analysis-PySpark.git
   cd ICICI-Bank-Stock-Analysis-PySpark

   Install Dependencies

Python 3.x

Apache Spark installed & configured

PySpark:
pip install pyspark
Prepare the Dataset

Place the ICICIBANK.csv file in the root/project folder.

Run the Analysis

Open Jupyter Notebook or VSCode.

Run the .ipynb or .py files in order to follow the analysis workflow.

📊 Tools & Technologies Used
Language: Python 3.x

Framework: Apache Spark (PySpark)

Libraries: pyspark.sql, pyspark.sql.functions, SQL queries, Window functions

Platform: Jupyter Notebook 

📌 Conclusion
This project demonstrates how PySpark can be applied to financial datasets for efficient large-scale data processing and analysis. 
It delivers practical insights that can assist in making informed investment decisions by analyzing historical stock trends, volatility, and trading behavior.
