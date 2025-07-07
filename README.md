# 🧠 Cryptocurrency Historical Prices Analysis

## 📌 Overview

This project explores and analyzes historical price data of various cryptocurrencies. The dataset is sourced from Kaggle and includes daily prices, volume, and market movements of hundreds of digital tokens.

## 🎯 Project Objectives

- Combine and clean historical data from multiple cryptocurrency files.
- Perform descriptive statistical analysis including mean, median, max, and standard deviation.
- Identify top-performing tokens by price and explore volatility.
- Visualize trends across popular altcoins.

## 📂 Dataset Source

[Kaggle - Cryptocurrency Historical Prices (Updated Daily)](https://www.kaggle.com/datasets/sudalairajkumar/cryptocurrencypricehistory)

Each CSV file contains historical data for a specific token, including:

- `Date`
- `Open`, `High`, `Low`, `Close`, `Adj Close`
- `Volume`

## 🛠 Tools & Libraries

- Python 3
- Pandas
- Plotly Express
- glob / os (for file handling)

## 📊 Workflow Summary

1. **Import and Merge** CSV files from folder using `glob`.
2. **Extract Token Info**: Derive `Symbol` from filenames (e.g., `"BTC_Bitcoin.csv"` → `BTC`).
3. **Data Cleaning**:
   - Remove rows with negative or zero values.
   - Convert `Date` to datetime, ensure numeric types for calculations.
4. **Statistical Analysis**:
   - Mean, Median, Max, Min, and Standard Deviation per token.
5. **Visualization**:
   - Highest Recorded Prices
   - Top Average Prices
   - Trends of Selected Altcoins
6. **Insights**:
   - Tokens like `SOCKS` have extremely high average prices due to scarcity-based valuation, not market cap.
   - Tokens with `NaN` or zero standard deviation indicate flat price behavior.

## 📈 Example Visualizations

- **Price Trends for Popular Altcoins**  
  *![line charts of closing prices over time](popular-altcoin-trend.png)*

- **Top 10 Most Volatile Tokens**  
  *![bar charts of top tokens for volatility](top-10-most-volatile-tokens.png)*