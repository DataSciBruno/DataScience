# Stock Price Prediction based on Trend
This repository contains a Python script for analyzing stock trends using historical data obtained from Yahoo Finance. The script utilizes various libraries such as yfinance, numpy, pandas, matplotlib, and statistics to perform the analysis.

## Libraries
The following libraries are imported in the script:

import yfinance as yf
import numpy as np
import pandas as pd
import random
import matplotlib.pyplot as plt
import statistics

## Getting the Data
The script defines a function historical_data(ticker) to download historical stock data for a given ticker symbol using the yfinance library. An example usage of the function is shown below:

ticker = input("Enter stock ticker: ")
data = historical_data(ticker)

## Preparation
The downloaded data is stored in the data variable. The script performs some data preparation steps, including the creation of a percentage change column, filling missing values using a rolling mean, and adding additional features such as volatility, RSI, Bollinger Bands, and exponential moving averages (EMAs).

## Establishing Trend
The script establishes the stock trend based on the comparison between the 50-day simple moving average (SMA) and the 200-day SMA. The Trend column is created, representing whether the stock is in an uptrend or a downtrend.

## Interval Analysis
The script identifies intervals of consecutive rows where the stock is in a downtrend or an uptrend. It calculates the total length of the downtrend and uptrend intervals and determines the trend ratio by dividing the length of the uptrend by the length of the downtrend.

## Downward Trend Analysis
The script extracts the rows corresponding to each downtrend interval and stores them in a separate DataFrame. It also appends a new row with a high value to help visualize the downward trend intervals.

## Upward Trend Analysis
Similarly, the script extracts the rows corresponding to each uptrend interval and stores them in a separate DataFrame. It also appends a new row with a high value to help visualize the upward trend intervals.

## Machine Learning and Forecast
The script also includes machine learning techniques to forecast the stock's future trend. It divides the historical data into intervals based on the established trends (uptrend or downtrend) and calculates the total length of each trend.

The intervals_down and intervals_up variables store the start and end indices of the downtrend and uptrend intervals, respectively. The lengths of these intervals are calculated and used to compute the trend ratio.

Next, the script creates two DataFrames, d_trend_adj and up_trend_adj, which store the adjusted closing prices of the intervals for downtrends and uptrends, respectively. These DataFrames can be used for further analysis and forecasting.

Finally, the script utilizes machine learning techniques to forecast future trends based on the available data. Please note that the specific machine learning algorithms and methods for forecasting are not mentioned in the provided code snippet.

## Conclusion
This script provides a comprehensive analysis of historical stock data, including trend analysis, technical indicator calculations, and the potential for forecasting using machine learning techniques. It serves as a useful tool for understanding stock trends and making informed investment decisions.

Feel free to modify and extend this script based on your specific requirements.

## Acknowledgements
This script was developed using Python and various open-source libraries, including yfinance, numpy, pandas, and matplotlib. Special thanks to the authors and contributors of these libraries for their valuable contributions to the open-source community.

## Disclaimer
This script is provided for educational and informational purposes only. It does not constitute financial advice or a recommendation to buy or sell any stocks. Always conduct thorough research and consult with a qualified financial advisor before making any investment decisions. Use this script at your own risk.
