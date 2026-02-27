# Trader Behavior vs Market Sentiment Analysis
### Junior Data Scientist – Trader Behavior Insights
Author: Ritik Rajput

---

## 📌 Objective

The objective of this project is to analyze whether trader performance and behavior vary across different market sentiment regimes (Fear vs Greed).

We evaluate:
- Profitability (PnL)
- Win rate
- Trade frequency
- Position size (risk appetite)
- Long/Short behavior

The goal is to derive actionable trading insights based on sentiment-driven behavioral patterns.

---

## 📊 Datasets Used

### 1️⃣ Bitcoin Market Sentiment Dataset
- Columns: Date, Classification (Fear, Greed, Extreme Fear, Extreme Greed, Neutral)
- Frequency: Daily

### 2️⃣ Historical Trader Data (Hyperliquid)
Includes:
- Account
- Execution Price
- Size (USD & Tokens)
- Side (BUY/SELL)
- Closed PnL
- Timestamp

---

## 🧹 Data Preparation

Steps performed:

1. Loaded both datasets using Pandas.
2. Cleaned column names to remove hidden spaces.
3. Converted timestamps to datetime format.
4. Extracted daily date from trade timestamps.
5. Aligned both datasets at daily level.
6. Merged sentiment data with trade data.
7. Created derived metrics:
   - Daily PnL per account
   - Win indicator
   - Average trade size
   - Trade count per sentiment
   - Long/Short ratio

Missing sentiment rows after merge: 6 (negligible).

---

## 📈 Analysis Performed

### 1️⃣ Performance Comparison
- Average PnL by sentiment
- Median PnL
- Win rate
- Trade count

### 2️⃣ Behavioral Analysis
- Average position size by sentiment
- Long/Short trade distribution
- Trade frequency differences

### 3️⃣ Trader Segmentation
- High vs Low position size traders
- Performance comparison across sentiment regimes

---

## 🔍 Key Insights

1. **Extreme Greed shows the highest average profitability and win rate.**
2. Traders take the **largest position sizes during Fear periods**, indicating aggressive dip-buying behavior.
3. Win rate declines significantly during Extreme Fear.
4. Selling dominates across most sentiment regimes, including Extreme Greed.

These findings suggest that trader performance and risk-taking behavior are sentiment-sensitive.

---

## 💡 Strategy Recommendations

1️⃣ During Extreme Fear:
- Reduce position size
- Apply stricter risk management
- Avoid aggressive averaging

2️⃣ During Extreme Greed:
- Apply trend-following strategies
- Maintain disciplined position sizing
- Consider momentum-based exposure

Sentiment-aware risk control improves trading robustness.

---

## ▶️ How to Run

1. Clone the repository
2. Install required libraries:
   - pandas
   - numpy
   - matplotlib
3. Open and run the notebook:
   `notebook.ipynb`

---

## 📌 Conclusion

This study confirms that market sentiment significantly influences trader behavior and profitability. Incorporating sentiment-aware adjustments into trading strategies can enhance performance stability and reduce downside risk.

---

Thank you for reviewing this submission.
