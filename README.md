# Stock Risk and Return Analysis
A Python-based project analyzing the relationship between stock returns and risk using real market data.

## 1. Problem & Target User
This project aims to help beginner investors understand how to evaluate stocks based on both return and risk, rather than focusing only on price changes.

The target users are beginner investors, especially university students who are new to stock investing.

## 2. Data
The dataset contains daily adjusted closing prices for 10 major technology companies over a one-year period.

- Source: Yahoo Finance
- Access date: 18 April 2026
- Key fields: Date (index), Adjusted closing prices for 10 stocks (AAPL, MSFT, NVDA, TSLA, AMZN, GOOGL, META, NFLX, AMD, INTC)

The data is stored locally as a CSV file and represents real historical market data.

## 3. Methods
The analysis is conducted using Python with the following steps:

- Load stock price data from CSV file
- Clean data and check for missing values
- Calculate daily returns using percentage change (pct_change)
- Compute average returns for each stock
- Measure volatility (risk) using standard deviation of daily returns
- Calculate Sharpe ratio to evaluate risk-adjusted performance
- Visualize price trends and risk-return relationship
- Rank stocks based on return, risk, and Sharpe ratio

These steps allow for a comprehensive comparison of stock performance from both return and risk perspectives.

## 4. Key Findings
- Stock price trends vary significantly across companies, reflecting differences in growth potential and market performance
- A clear positive relationship between risk and return is observed, indicating that higher returns generally come with higher volatility
- Some stocks (e.g., large-cap firms) exhibit more stable performance with relatively lower risk
- High-growth stocks tend to show both higher returns and higher fluctuations
- Investors should balance risk and return rather than focusing solely on maximizing returns
- For example, some stocks achieve higher returns but also exhibit higher volatility in the risk-return analysis plot
- Risk-adjusted performance (measured by the Sharpe ratio) provides a more comprehensive evaluation of stock attractiveness

## 5. How to Run
1. Install required libraries:
   ```
   pip install pandas numpy matplotlib yfinance
   ```
2. Download or clone this repository

3. Open the Jupyter Notebook:
ACC102_Stock_Risk_Return_Analysis.ipynb

4. Run all cells to reproduce the analysis

## 6. Demo / Output

The project produces the following outputs:

- Stock price trend visualization over time
- Daily return calculations for each stock
- Risk vs Return scatter plot
- Stock ranking based on return, risk, and Sharpe ratio

These outputs can be viewed directly in the Jupyter Notebook after running the code.

## 7. Limitations & Future Improvements
- The analysis only considers historical price data and does not include macroeconomic factors
- Only 10 stocks are analyzed, which may limit generalizability
- Future work could include:
- More industries or stocks
- Portfolio optimization
- Inclusion of financial indicators
- Use of additional risk-adjusted metrics
