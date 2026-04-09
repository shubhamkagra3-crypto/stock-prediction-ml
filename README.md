# 📈 HDFC Bank Stock Prediction (ML Project)

This project uses machine learning to predict short-term price movement of **HDFC Bank (HDFCBANK.NS)** using historical stock data and technical indicators.

---

## 🎯 Goal

Predict whether the next day price will increase by more than **0.5%** using past market data.

---

## 📊 Dataset

- Source: Yahoo Finance (`yfinance`)
- Stock: HDFC Bank (HDFCBANK.NS)
- Time Range: 2018 – 2025

---

## ⚙️ Features Used

- Trend
- MA_diff
- Momentum_3
- Momentum_5
- Volatility
- Range
- Volume_Spike
- Body_Ratio
- Breakout

---

## 🎯 Target

```python
data['Target'] = (data['Return'].shift(-1) > 0.005).astype(int)


🤖 Model
Random Forest Classifier (Scikit-learn)
Time-series train-test split (80/20)
📊 Result
Accuracy: ~0.58 – 0.60
⚠️ Note

This project is for learning purposes only, not financial advice.