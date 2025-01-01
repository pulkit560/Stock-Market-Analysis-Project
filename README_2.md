# Stock Market Prediction and Trading Strategy

## Table of Contents
1. [Project Overview](#project-overview)
2. [Data Description](#data-description)
3. [Setup and Installation](#setup-and-installation)
4. [Implementation Steps](#implementation-steps)
5. [Results and Performance](#results-and-performance)
6. [Evaluation Metrics](#evaluation-metrics)
7. [Conclusion](#conclusion)
8. [References](#references)

---

## Project Overview
This project demonstrates a trading strategy based on a **multiple linear regression model** to predict the SPY stock price using historical data from various global stock markets. The primary objective is to generate actionable signals and evaluate the strategy's profitability against traditional buy-and-hold approaches.

---

## Data Description
The project uses historical data from the following stock indices:
- **SPY** (S&P 500 ETF)
- **SP500** (S&P 500 Index)
- **NASDAQ** (Nasdaq Composite Index)
- **DJI** (Dow Jones Industrial Average)
- **CAC40** (French CAC 40 Index)
- **DAXI** (German DAX Index)
- **AORD** (Australian All Ordinaries)
- **HSI** (Hong Kong Hang Seng Index)
- **NIKKEI** (Japanese Nikkei 225)

Each dataset contains:
- Opening and closing prices
- Adjustments to remove timezone discrepancies

---

## Setup and Installation

### Prerequisites
Ensure the following libraries are installed:
- `pandas`
- `numpy`
- `statsmodels`
- `matplotlib`

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo/stock-prediction-strategy.git
   cd stock-prediction-strategy

   # Trading Strategy Based on SPY and S&P 500
---
## Implementation Steps

### 1. Data Preprocessing
- Load the datasets `SPY.csv` and `SP500.csv`.
- Handle missing values using forward fill and remove remaining NaNs.
- Calculate daily changes in the indices to create features.
- 
### 2. Feature Engineering
- Create lag variables to capture temporal dependencies.
- Combine datasets into a single dataframe for analysis.

### 3. Data Splitting
- Split the dataset into training and test sets.

  ### 4. Model Building
- Build a multiple linear regression model using statsmodels.
- 
### 5. Signal-Based Trading Strategy
- Generate buy/sell signals based on model predictions.
- Simulate trading performance and compare with a buy-and-hold strategy.

---
## Results

The strategy's cumulative wealth is compared against a buy-and-hold strategy. 

---

## Future Scope
- Explore additional features for better signal accuracy.
- Implement advanced forecasting techniques (e.g., ARIMA, LSTM).
- Automate the entire pipeline for real-time trading.

