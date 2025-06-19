# 📈 Stock Market Analysis & Apple Stock Price Prediction using LSTM

This project analyzes historical stock data of major tech companies—**Apple (AAPL), Google (GOOG), Microsoft (MSFT), and Amazon (AMZN)**—over the past year using data from **Yahoo Finance**. It then uses **LSTM (Long Short-Term Memory)**, a deep learning algorithm, to **predict Apple's stock closing prices**.

## 📊 Features

- 📥 Fetches real-time historical stock data using `yfinance`
- 📉 Visualizes:
  - Closing prices
  - Daily returns
  - Moving averages (10, 20, 50 days)
  - Volume trends
  - Correlation heatmaps
- 🧠 Predicts Apple's stock prices using LSTM Neural Network
- 📈 Calculates RMSE to evaluate prediction accuracy

---

## 🛠️ Tech Stack

- **Languages**: Python
- **Libraries**: 
  - `yfinance`
  - `pandas`, `numpy`
  - `matplotlib`, `seaborn`
  - `scikit-learn`
  - `keras` (with TensorFlow backend)

---

## 📦 Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/stock-analysis-lstm.git
   cd stock-analysis-lstm
