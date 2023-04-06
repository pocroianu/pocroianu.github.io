---
title: "Stock Trading Bot with Machine Learning"
date: 2023-04-06
draft: false
tags: ["Machine Learning", "Trading", "Python"]
---

In this blog post, we will walk through the process of building a stock trading bot using machine learning techniques. We will cover the following topics:

- Fetching historical stock data
- Feature engineering using technical indicators
- Training and evaluating machine learning models
- Generating buy/sell signals
- Executing trades

## Fetching Historical Stock Data

We use the `yfinance` library to fetch historical stock data. The `fetch_data` function downloads the historical data for a single stock, while the `fetch_data_multiple` function downloads the data for multiple stocks.

\```python
import yfinance as yf

def fetch_data(symbol, start, end):
    # ...

def fetch_data_multiple(symbols, start, end):
    # ...
\```

## Feature Engineering with Technical Indicators

We use the `talib` library to calculate technical indicators for our dataset. The `preprocess_data` function calculates several indicators like moving averages, Bollinger Bands, RSI, MACD, and others, which are used as features for our machine learning model.

\```python
import talib

def preprocess_data(df):
    # ...
\```

## Training and Evaluating Machine Learning Models

We use the `sklearn` library to train and evaluate Gradient Boosting Regressor models. We perform hyperparameter tuning using `GridSearchCV`. The `train_model` function trains a single model, while the `train_models` function trains multiple models for multiple stocks.

\```python
from sklearn.ensemble import GradientBoostingRegressor
from sklearn.model_selection import GridSearchCV

def train_model(df):
    # ...

def train_models(data):
    # ...
\```

## Generating Buy/Sell Signals

We generate buy/sell signals for each stock using the trained models. The `generate_signals` function predicts the next day's closing price and compares it to the current closing price to determine whether to buy or sell the stock.

\```python
def generate_signals(models, feature_names, data):
    # ...
\```

## Executing Trades

We use the Alpaca API to execute trades

\```python
def execute_trades(signals):
    # ...
\```
