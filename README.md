# Stock-Price-Prediction

Stock Price Analysis and Prediction
Project Overview
This project analyzes historical stock price data for major tech companies (Apple, Google, Microsoft, Amazon) and predicts Apple's future stock prices using an LSTM neural network. The analysis includes visualizations of trading volumes, moving averages, daily returns, and correlations, with predictive modeling to forecast Apple's closing prices.
Features

Data Collection: Fetches historical stock data using the yfinance library for the past year.
Visualizations:
Plots of daily trading volumes for each company.
Moving averages (10, 20, 50 days) for stock closing prices.
Daily return percentage plots and histograms.
Correlation analysis with heatmaps and pair plots.


Prediction Model:
Uses an LSTM neural network to predict Apple's stock prices.
Trains on 95% of historical data (2012–2023) and tests on the remaining 5%.


Performance Metrics: Calculates RMSE as a percentage of the average closing price.

Requirements

Python 3.x
Libraries:
yfinance
pandas
numpy
matplotlib
seaborn
keras
scikit-learn



Install dependencies using:
pip install yfinance pandas numpy matplotlib seaborn keras scikit-learn

Usage

Clone the Repository:
git clone <repository_url>
cd <repository_directory>


Run the Script:

Execute the main Python script (e.g., stock_analysis.py) in a Jupyter notebook or Python environment.
Ensure you have an internet connection for yfinance to fetch stock data.


Expected Outputs:

Dataframes with stock data for AAPL, GOOG, MSFT, AMZN.
Visualizations (saved or displayed) for volume, moving averages, daily returns, and correlations.
Predicted Apple stock prices with RMSE evaluation.



Data

Source: Yahoo Finance via yfinance.
Time Period:
General analysis: Past 1 year (from current date).
Prediction model: 2012–2023 for Apple (AAPL).


Features Used:
Closing prices, trading volumes, moving averages, daily returns.
Scaled closing prices for LSTM input.



Model Architecture

LSTM Model:
Two LSTM layers (128 and 64 units).
Two Dense layers (25 units and 1 unit for output).
Trained with Adam optimizer and mean squared error loss.
Input: 60-day sequences of scaled closing prices.
Output: Predicted closing price for the next day.



Results

Visualizations: Provide insights into stock trends, volatility, and correlations.
Prediction Performance:
RMSE as a percentage of average closing price: ~11.58%.
Predictions are based on historical patterns and may not account for external market factors.



Limitations

The model relies on historical data and may not capture sudden market changes.
yfinance data may have occasional gaps or inconsistencies.
LSTM predictions assume stationarity in patterns, which may not always hold.

Future Improvements

Incorporate additional features (e.g., technical indicators, sentiment analysis).
Experiment with other models (e.g., ARIMA, Transformer-based models).
Extend the analysis to include real-time data or more companies.

License
This project is licensed under the MIT License.
Acknowledgments

Data provided by Yahoo Finance via yfinance.
Built with Python, Keras, and data visualization libraries.

