# Development of an Automated GBP/USD Forex Trading Bot Using ML

## Project Overview

This project aims to develop an automated trading system for the Forex market using machine learning models. The system predicts future prices of the GBP/USD currency pair and generates trading signals to execute buy and sell orders. The project explores various machine learning models, including Gated Recurrent Unit (GRU), Extreme Gradient Boosting (XGBoost), and Random Forest, and compares their performance.

**Research Question**: How can machine learning algorithms be used to develop a profitable
automated trading bot for the GBP/USD Forex market using GRU, XGBOOST,
and Random Forest models?

## Data Description
- **Source**: Yahoo Finance
- **Fields**: Date, Open, Close, High, Low, Adj close prices, Volume
- **Technical Indicators**: EMAs, RSI, MACD

## Project Structure

- **Data Collection**
  - Forex price history timeframe: December 2003 to May 2024
- **Data Preparation**
  - Data Cleaning and Preprocessing:
    - Inspect dataset, drop missing values, drop irrelevant columns, normalize data
  - Feature Engineering:
    - Calculate EMA (20, 50), RSI (14), MACD (12, 26, 9)
- **Model Development**
  - Data Preparation for Modeling:
    - Split dataset, create sequences, scale data
  - Model Selection and Training:
    - Train GRU, XGBoost, and Random Forest models
  - Hyperparameter Tuning:
    - Optimize model performance for XGBoost and Random Forest
- **Model Evaluation**
  - Performance Metrics
- **Trading Strategy**
  - Strategy Development and Rules
  - Simulation Results and Performance Metrics
- **Discussion**
  - Interpretation of Results
  - Comparison with existing methods and literature
  - Limitations and Potential Improvements
- **Conclusion**
  - Summary of Findings
  - Future Work and Directions

## Key Features

- **Data Cleaning and Preprocessing**: Cleaning the dataset by removing missing values and irrelevant columns. Normalizing the data to prepare it for modeling.
- **Feature Engineering**: Creating technical indicators such as EMA, RSI, and MACD to use as features in the models.
- **Model Development**: Developing and training three machine learning models (GRU, XGBoost, Random Forest) to predict future Forex prices.
- **Model Evaluation**: Evaluating the models using performance metrics such as MSE, MAE, RMSE, R2, and MAPE.
- **Trading Strategy**: Implementing a trading strategy based on the model predictions, including rules for buy/sell signals, stop-loss, and take-profit mechanisms.
- **Performance Comparison**: Comparing the trading performance of individual models and an ensemble model in terms of final balance, profit, Sharpe ratio, and maximum drawdown.
- **Visualization**: Plotting predictions, residuals, and trading performance to visualize the results.

## Results

The project evaluates the performance of the models based on various metrics and implements a trading strategy to simulate trades. The ensemble model, combining predictions from GRU, XGBoost, and Random Forest, shows the best overall performance in terms of profit and risk management.

## Requirements

- Python 3.x
- Libraries: pandas, numpy, scikit-learn, keras, xgboost, matplotlib

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/Cynthiaudoye/Forex_Trading_Bot.git

