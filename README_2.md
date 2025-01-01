SPY Trading Strategy Using Multiple Linear Regression
Overview
This project demonstrates the development of a trading strategy for SPY (an ETF tracking the S&P 500 index) using multiple linear regression. The model leverages historical data from various stock indices to predict SPY price movements, enabling a signal-based trading strategy.

Key Objectives
Build a predictive model to estimate SPY price changes based on other stock indices' data.
Evaluate the model's performance using both statistical and practical metrics.
Compare the profitability of a signal-based strategy with a traditional "buy-and-hold" approach.
Data Sources
The project uses historical data from the following stock markets:

ALLOrdinary (AORD)
Nikkei 225 (Japan)
Hang Seng Index (HSI)
DAX Index (Germany)
CAC40 (France)
S&P 500 (SP500)
Dow Jones Industrial Average (DJI)
NASDAQ Composite
SPY ETF (S&P 500 tracker)
Workflow
Step 1: Data Preparation
Data Cleaning: Handle missing values using forward filling and drop remaining NaN values.
Feature Engineering: Create lagged and difference features to capture historical trends:
Example: SPY price difference (spy) and lagged SPY (spy_lag1).
Save the cleaned and processed dataset (indicepanel.csv) for further analysis.
Step 2: Data Splitting
Training Set: 1,000 data points from the earlier part of the dataset.
Test Set: 1,000 data points from the latter part of the dataset.
Step 3: Exploratory Analysis
Scatter Matrix: Visualize relationships between SPY and other indices.
Correlation Analysis: Identify indices with the highest correlation to SPY price changes.
Step 4: Model Building
Regression Formula:
spy ~ spy_lag1 + sp500 + nasdaq + dji + cac40 + aord + daxi + nikkei + hsi
Use the Ordinary Least Squares (OLS) method to estimate model parameters.
Step 5: Predictions
Generate predictions for both the training and test datasets.
Evaluate the model's predictions with scatterplots and statistical metrics.
Evaluation Metrics
Statistical Metrics
Adjusted $R^2$: Measures the goodness-of-fit, adjusted for the number of predictors.
RMSE (Root Mean Squared Error): Quantifies prediction errors.
Practical Metrics
Sharpe Ratio:
Measures risk-adjusted returns (daily and annualized).
Maximum Drawdown:
Assesses the maximum observed loss during the strategy's run.
Strategy Performance
Signal-Based Trading: Generate buy/sell signals based on predicted price changes.
Comparison: Compare cumulative wealth from the signal-based strategy to a buy-and-hold approach.
Results
Training Set
Total Profit: X (Insert result)
Sharpe Ratio: Daily: X, Yearly: X
Maximum Drawdown: X%
Test Set
Total Profit: X (Insert result)
Sharpe Ratio: Daily: X, Yearly: X
Maximum Drawdown: X%
