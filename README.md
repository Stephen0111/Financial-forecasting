# Financial-forecasting
Stock Price Forecasting & Sentiment Impact Analysis
Project Overview

This project demonstrates how financial news sentiment influences stock price movements across multiple tickers (AAPL, MSFT, GOOGL).
It combines:

Web scraping of Yahoo Finance news headlines

Sentiment analysis using VADER

Historical stock price data using yfinance

Feature engineering (returns, moving averages, volatility)

Time-series forecasting using Facebook Prophet

Model comparison to evaluate the impact of sentiment on predictive accuracy

The project is designed to showcase a junior data scientist’s end-to-end workflow: data collection, cleaning, feature engineering, modeling, visualization, and evaluation.
# Data Sources
| Data Type                | Source                           |
| ------------------------ | -------------------------------- |
| Stock OHLCV Prices       | `yfinance` API                   |
| Financial News Headlines | Yahoo Finance (scraping)         |
| Sentiment Scores         | VADER SentimentIntensityAnalyzer |

# 🧰 Tech Stack

Python 3.x

Jupyter Notebook

yfinance

BeautifulSoup4 & requests

VADER SentimentAnalysis

Prophet (Facebook Prophet)

Matplotlib & Plotly

# 🛠️ Project Workflow

Data Collection

Scrape financial news headlines and timestamps for multiple tickers

Fetch historical stock prices (OHLCV) using yfinance

Data Cleaning & Merging

Remove duplicates and clean timestamps

Compute sentiment scores for headlines

Aggregate daily sentiment per ticker and combined

Merge sentiment scores with stock prices

Feature Engineering

Compute daily returns

Calculate moving averages (7-day, 30-day)

Calculate rolling volatility

Compute sentiment rolling averages

Time-Series Forecasting

Prophet baseline model (price only)

Prophet model with sentiment as regressor

Forecast next 30 days

Evaluation & Comparison

RMSE comparison of baseline vs sentiment-enhanced models

Visualize sentiment trends per ticker and combined

Display 30-day forecasts for all tickers

# 💡 Key Learnings

Demonstrates how news sentiment can improve time-series forecasts

Highlights multi-ticker data processing and merging

Shows end-to-end workflow from web scraping → sentiment → feature engineering → forecasting → evaluation

Provides clean, professional visualizations suitable for a portfolio
