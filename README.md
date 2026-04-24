# Stock Risk and Return Analysis
This project uses Python to analyze stock performance based on return and risk using real financial data from WRDS. It focuses on helping users compare different stocks and understand how risk and return are related.

## 1. Problem & Target User
This project aims to help users understand how to evaluate stock performance using both return and risk, rather than relying only on price movements.

The target users are university students who have some basic knowledge of finance but find it difficult to apply it in practice, as well as beginners who have little or no prior knowledge of financial analysis.


## 2. Data
The dataset contains daily stock price data for 10 major technology companies over a one-year period.

- Source: WRDS – CRSP database  
- Access method: Python connection using a WRDS account  
- Access date: 22 April  2026  

Key fields:
- date: trading date  
- permno: stock identifier  
- prc: stock price  

The selected companies include large technology firms such as AAPL, MSFT, NVDA, TSLA, AMZN, GOOGL, META, NFLX, AMD, and INTC.


## 3. Methods
The analysis is implemented as a reusable Python function, allowing flexible user input.

Main steps:
• Connect to WRDS using a user-provided username  
• Retrieve stock price data based on selected tickers  
• Convert data into a structured time-series format  
• Calculate daily returns using percentage change (pct_change)  
• Compute key performance metrics:
  - Average return  
  - Volatility (standard deviation of returns)  
  - Sharpe ratio (risk-adjusted return)  
  - Visualize results using different plots  

This structure makes the analysis more flexible, as users can easily change inputs such as tickers and time period without modifying the main logic of the code.

## 4. Key Findings
- Stock performance differs noticeably across companies, suggesting that firm-specific factors play an important role beyond general market trends
- A positive relationship between risk and return is generally observed, but the strength of this relationship varies across different stocks
- Some stocks achieve higher returns but also exhibit significantly higher volatility, indicating less stable performance
- Stocks with moderate returns and lower volatility tend to provide more consistent performance over time
- The Sharpe ratio shows that higher returns do not always imply better performance when risk is taken into account

## 5. How to Run
1. Install required libraries:
   ```
   pip install pandas numpy matplotlib wrds
   ```
2. Download or clone this repository

3. Open the Jupyter Notebook:
ACC102_Stock_Risk_Return_Analysis.ipynb

4. Run all cells to reproduce the analysis

## 6. Demo / Output

The project produces the following outputs:
- Stock price trend visualization over time
- Daily return calculations for each stock
- Cumulative return comparison across stocks
- Stock ranking based on return, risk, and Sharpe ratio
These outputs can be viewed directly in the Jupyter Notebook after running the code.

## 7. Limitations & Future Improvements
- The analysis is based only on historical price data and does not include macroeconomic or firm-specific factors
- Only 10 stocks are analyzed, which may limit the generalizability of the results
- Future work could include:
- Expanding the number of stocks or industries
- Applying portfolio optimization techniques
- Incorporating additional financial indicators
- Using more advanced risk-adjusted performance measures
