# Financial-Analytics-Project-IITJ
Financial Analytics Project - IIT Jodhpur Project 

Detailed Report for Portfolio Analysis of Indian Stocks
This report provides a detailed analysis of a portfolio consisting of 10 Indian stocks. 
The analysis includes calculating stock returns, correlations, descriptive statistics, 
and the creation of a combined index. Additionally, the report discusses the Markowitz 
Efficient Frontier, Capital Market Line (CML), and Security Market Line (SML) for optimizing 
portfolio returns and risk. The combined index return and risk are also calculated.

1. Importing Libraries
The following libraries are imported to perform data analysis and visualization:
- yfinance: To download financial data for the selected assets.
- pandas: To handle and manipulate the data.
- numpy: To perform numerical calculations.
- matplotlib and seaborn: For creating visualizations.
- scipy: Used for optimization tasks (although not explicitly used in this report).

2. Defining the Assets and Downloading Data
We have selected 10 Indian stocks to analyze. Their adjusted closing price data for the 
past three years (from January 1, 2021, to January 1, 2024) is downloaded using the yfinance
library.

3. Calculating Daily Returns
Daily returns are calculated using the percentage change in the adjusted closing price 
using the pandas function pct_change(). The first row is dropped using dropna() to handle missing
values.

4. Plotting Asset Data (Time Series and Histogram)
We define a function that plots the time series of asset prices and the histogram of 
daily returns for each asset. The time series shows how the price evolves over time, 
while the histogram helps visualize the distribution of daily returns.

5. Calculating Descriptive Statistics
Descriptive statistics are calculated for each asset using pandas describe(). 
The statistics include mean, standard deviation, skewness, and kurtosis, 
which give insights into the distribution of returns.

6. Correlation Analysis
The correlation matrix of asset returns is calculated to understand how assets move relative to each
other. 
A heatmap is generated to visualize the correlations between the assets.

7. Creating a Combined Index
A combined index is created by calculating the weighted average of the daily returns of all selected
assets. 
The cumulative returns of this weighted index are calculated, which represents the performance of
the combined portfolio.

8. Markowitz Efficient Frontier, CML, and SML
The Markowitz Efficient Frontier is calculated by generating random portfolios and plotting their
return and risk. 
The portfolio with the maximum Sharpe ratio is identified as the Market Portfolio. 
The Capital Market Line (CML) is plotted to show the optimal risk-return trade-off, 
and the Security Market Line (SML) is plotted for a selected asset (RELIANCE.NS).

9. Combined Index Return and Risk
The return and risk (volatility) of the combined index are calculated and annualized.
These values provide an overview of the overall performance of the portfolio.

#Conclusion
This report successfully analyzes the portfolio consisting of 10 Indian stocks. 
It includes the calculation of returns, risks, correlations, and descriptive statistics. 
By using the Markowitz Efficient Frontier, Capital Market Line, and Security Market Line, 
we can determine the optimal portfolio and expected return for a selected asset.
