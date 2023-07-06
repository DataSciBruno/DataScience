# Time Series Analysis for Stock Price
This project focuses on conducting time series analysis for stock price data. Various indicators and statistical measures are calculated to gain insights into the behavior of the stock price over time.

## Libraries
The following libraries are used in this project:

numpy: For numerical computations.

pandas: For data manipulation and analysis.

yfinance: For downloading stock price data.

datetime: For handling dates.

matplotlib.pyplot: For data visualization.

mplfinance: For plotting OHLC (Open, High, Low, Close) charts.

## Dataset
You will be prompted to enter the stock ticker symbol and the start date for the data. The yfinance library is used to download the historical stock price data.

## Calculating Indicators
The following indicators and statistical measures are calculated:

Returns: The percentage change in the adjusted closing price from the previous day.

Log Returns: The logarithmic returns, which often exhibit a more symmetric and approximately normal distribution compared to regular returns.

Historical Volatility: The volatility of returns calculated using the rolling standard deviation.

Exponential Moving Averages (EMA): EMA values are calculated for different periods (8, 21, 50, 72, 144, and 200).

Relative Strength Index (RSI): A momentum oscillator that measures the speed and change of price movements.

Bollinger Bands: A volatility indicator that consists of a moving average and upper/lower bands based on standard deviations.

## Visualization
The calculated indicators are plotted using various visualization techniques:

OHLC Chart: A candlestick chart that shows the Open, High, Low, and Close prices for each day.

EMA Indicators: The EMA values are plotted on the chart.

RSI Indicator: The RSI values are plotted on the chart.

Bollinger Bands: The upper and lower Bollinger Bands are plotted on the chart.

Please note that this project serves for educational purposes and should not be considered as financial advice.

Feel free to explore the provided code and modify it according to your requirements. Have fun analyzing stock price data using time series techniques!
