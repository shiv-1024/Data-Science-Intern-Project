# Data-Science-Intern-Project

📊 Trader Behavior & Sentiment Analysis
📌 Project Overview

This project analyzes trader performance and behavioral patterns under different market sentiment regimes (Fear vs Greed).

The objective is to:

Compare trader performance across sentiment regimes

Detect behavioral changes (trade frequency, position size, bias)

Segment traders into meaningful categories

Propose data-driven strategy rules

The dataset contains executed trade data including PnL, position size, sentiment classification, and trader identifiers.

📁 Dataset Description

Main columns used:

Column	Description
Account	Trader identifier
Trade ID	Unique trade ID
Closed PnL	Profit/Loss per trade
Size USD	Trade position size in USD
classification	Market sentiment (Fear / Greed)
Side	Long / Short
date	Trade date
Execution Price	Trade execution price
🎯 Project Goals
1️⃣ Performance Analysis

Total PnL by sentiment

Average PnL

Win rate

Drawdown proxy (PnL volatility)

2️⃣ Behavioral Analysis

Trade frequency per day

Position size changes

Long/Short bias shifts

3️⃣ Trader Segmentation

Frequent vs Infrequent traders

Consistent vs Inconsistent traders

Volatility-based profiling

4️⃣ Strategy Design

Regime-based position sizing

Capital allocation by trader segment

Risk control rules

📊 Key Metrics Computed
Performance Metrics

Total PnL

Average PnL

Win Rate = % of trades with positive PnL

PnL Standard Deviation (drawdown proxy)

Behavioral Metrics

Average trades per day

Average position size (USD)

Long/Short ratio

Segmentation Metrics

Total trades per trader

Win rate per trader

PnL volatility per trader

📈 Visualizations

The project includes:

Bar charts: Fear vs Greed performance

Boxplots: Position size distribution

Histograms: Win rate distribution

Trade frequency comparison

Long/Short bias by sentiment

Libraries used:

pandas

matplotlib

seaborn

🧠 Key Findings (Example Summary)

Performance differs between Fear and Greed regimes.

Trade frequency increases during Greed periods.

Position sizes tend to be larger in Greed environments.

Consistent traders outperform high-frequency inconsistent traders.

Volatility (drawdown proxy) increases in Fear regimes.

🚀 Strategy Rules Proposed
Rule 1 — Risk Adjustment by Sentiment

During Fear days:

Reduce position size

Restrict low win-rate traders

Focus on capital preservation

During Greed days:

Increase exposure selectively

Allocate more capital to consistent traders

Rule 2 — Segment-Based Capital Allocation

Allocate more capital to consistent traders

Cap risk for high-frequency inconsistent traders

Avoid scaling aggressive traders in Fear regimes

🛠 Implementation Workflow

Data cleaning and preprocessing

Feature engineering (win rate, volatility, segmentation)

Sentiment-based grouping

Visualization & analysis

Strategy simulation via adjusted position sizing

📦 How to Run
pip install pandas matplotlib seaborn

Open the notebook and execute all cells sequentially.

Ensure:

Closed PnL and Size USD are numeric

date column is datetime

🔮 Future Improvements

Add true leverage analysis (if margin data available)

Compute Sharpe ratio & Sortino ratio

Add cumulative equity curve

Perform rolling drawdown analysis

Add statistical significance testing

Convert to full backtesting framework

📌 Conclusion

This project demonstrates how trader performance and behavior shift across market sentiment regimes and how segmentation-based strategies can improve risk-adjusted returns.

The analysis highlights the importance of:

Regime-aware risk management

Behavioral profiling

Data-driven capital allocation
