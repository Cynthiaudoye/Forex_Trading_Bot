# Development of an Automated GBP/USD Forex Trading Bot Using ML

## Project Overview

This project aims to develop an automated trading system for the Forex market using machine learning models. The system predicts future prices of the GBP/USD currency pair and generates trading signals to execute buy and sell orders. The project explores various machine learning models, including Gated Recurrent Unit (GRU), Extreme Gradient Boosting (XGBoost), and Random Forest, and compares their performance.

**Research Question**: How can machine learning algorithms be used to develop a profitable automated trading bot for the GBP/USD Forex market using GRU, XGBOOST, and Random Forest models?

# Forex Market Prediction Project

## Data Ethics

This project ensures ethical compliance by utilizing publicly available data from Yahoo Finance, which does not include personal information, thus adhering to GDPR guidelines. All data usage aligns with Yahoo Finance's terms of service and the ethical guidelines of the University of Hertfordshire. 

The project maintains transparency and reproducibility through detailed documentation and version control on GitHub. Additionally, it emphasizes responsible research by thoroughly testing the automated trading bot to mitigate financial risks, ensuring that all findings are reported honestly and without manipulation.

It is important to note that the algorithm and trading bot are still under supervision and training, and it is not advised to use them for real money trading to avoid potential financial loss.

Furthermore, the project addresses ethical concerns such as market manipulation by implementing safeguards such as using technical indicators to ensure trades are based on real market conditions. It ensures transparency by providing clear and accessible information about the bot's algorithms and promotes accessibility and fairness by offering equal opportunities for all users.


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

## Usage

**Prepare the Dataset**: Ensure the dataset is in the appropriate directory.

**Data Preparation**: Run the data preparation script to clean and preprocess the data.

**Model Training**: Train the machine learning models by running the model development script.

**Model Evaluation**: Evaluate the models and generate trading signals using the evaluation script.

**Trading Simulation**: Simulate trades and analyze the performance of the trading strategy.

### Loading Saved Models

The pre-trained models are saved and uploaded to this directory in the repository. These include:

- `best_model_gru.keras`: The GRU model
- `best_model_xgb.json`: The XGBoost model
- `best_model_rf.pkl`: The Random Forest model

## Future Work and Directions

To further enhance the model's performance and robustness, future work could focus on:

- **Advanced Trading Strategies**: Implement and test more sophisticated trading strategies such as momentum-based trading, mean reversion strategies, and algorithmic trading.
- **Incorporating Additional Data**: Include macroeconomic indicators, news sentiment analysis, and other relevant data to improve model predictions.
- **Real-time Trading**: Develop the system for real-time trading to evaluate its performance in live market conditions.
- **Enhanced Risk Management**: Explore more advanced risk management techniques to optimize the trading strategy's performance.

## Acknowledgments

I would like to express my gratitude to my supervisor and colleagues for their support and guidance throughout this project. Special thanks to the open-source community for providing valuable resources and tools that made this project possible.

## Contact

For any questions or suggestions, please feel free to reach out to me at cindymary621@gmail.com.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue to discuss potential improvements or report bugs.

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/Cynthiaudoye/Forex_Trading_Bot.git
