# 📊 Trader Behavior & Market Sentiment Analysis

## 🚀 Overview

This project analyzes how trader performance and behavior change under
different market sentiment regimes (**Fear vs Greed**).

Using trade-level data, we evaluate:

-   📈 Performance differences (PnL, win rate, volatility)
-   🔄 Behavioral shifts (trade frequency, position size, long/short
    bias)
-   🧩 Trader segmentation (consistent vs inconsistent, frequent vs
    infrequent)
-   🧠 Strategy rules based on data-driven insights

The goal is to transform raw trade data into actionable trading
insights.

------------------------------------------------------------------------

## 📁 Dataset Features

  Column            Description
  ----------------- ---------------------------------
  Account           Trader identifier
  Trade ID          Unique trade identifier
  Closed PnL        Profit/Loss per trade
  Size USD          Trade size in USD
  classification    Market sentiment (Fear / Greed)
  Side              Long / Short
  date              Trade date
  Execution Price   Execution price
  Fee               Trading fee

------------------------------------------------------------------------

## 📊 Analysis Performed

### 1️⃣ Performance Analysis (Fear vs Greed)

-   Total PnL
-   Average PnL
-   Win Rate
-   PnL Volatility (Drawdown Proxy)

### 2️⃣ Behavioral Analysis

-   Trade frequency per day
-   Position size distribution
-   Long vs Short ratio by sentiment

### 3️⃣ Trader Segmentation

-   Frequent vs Infrequent traders
-   Consistent vs Inconsistent traders
-   Volatility-based risk profiling

------------------------------------------------------------------------

## 📈 Key Insights

### ✅ Insight 1 --- Performance Differs by Sentiment

Performance metrics show variation between Fear and Greed regimes,
including differences in win rate and volatility.

### ✅ Insight 2 --- Traders Become More Aggressive During Greed

Trade frequency and average position size increase during Greed periods.

### ✅ Insight 3 --- Consistent Traders Outperform

Traders with higher win rates exhibit more stable performance compared
to high-frequency inconsistent traders.

------------------------------------------------------------------------

## 🧠 Strategy Rules Proposed

### 📉 Rule 1 --- Risk Reduction During Fear

-   Reduce position size
-   Avoid scaling inconsistent traders
-   Prioritize capital preservation

### 📈 Rule 2 --- Selective Scaling During Greed

-   Increase exposure only for consistent traders
-   Limit aggressive, low win-rate traders
-   Maintain controlled expansion

------------------------------------------------------------------------

## 🛠 Tech Stack

-   Python
-   Pandas
-   Matplotlib
-   Seaborn
-   Jupyter Notebook

------------------------------------------------------------------------

## ▶ How to Run

``` bash
pip install pandas matplotlib seaborn
```

Open the notebook and run all cells.

------------------------------------------------------------------------

## 📌 Conclusion

This project demonstrates how:

-   Market sentiment influences trader performance
-   Behavioral metrics reveal risk patterns
-   Segmentation enables smarter capital allocation
-   Regime-aware strategies improve decision-making
