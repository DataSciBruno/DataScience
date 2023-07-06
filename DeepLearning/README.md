# Stock Price LSTM Model
This project focuses on building a Long Short-Term Memory (LSTM) model to predict stock prices. The LSTM model is a type of recurrent neural network (RNN) that is capable of learning long-term dependencies in sequential data.

## Libraries
The following libraries are used in this project:

pandas: For data manipulation and analysis.

numpy: For numerical computations.

sklearn.preprocessing.MinMaxScaler: For data normalization.

keras.models.Sequential: For creating a sequential model.

keras.layers.LSTM, keras.layers.Dropout, keras.layers.Dense: For defining LSTM layers, dropout regularization, and fully connected layers.

matplotlib.pyplot: For data visualization.

datetime: For handling dates.

yfinance: For downloading stock price data.

## Dataset
You will be prompted to enter the stock ticker symbol and the start date for the data. The yfinance library is used to download the historical stock price data.

## Preparation
The downloaded data is prepared for analysis by selecting only the 'Adj Close' column from the DataFrame.

## Stationarity
The stationarity of the time series data is evaluated using the Augmented Dickey-Fuller (ADF) test. The ADF test helps determine if the time series is stationary or not. Non-stationary data may exhibit trends or seasonality.

## Normalize
The data is normalized using the MinMaxScaler to ensure that all values fall within a specific range (typically between 0 and 1). Normalizing the data helps the LSTM model converge faster and improves its performance.

## Train & Test sizes
The data is split into train and test sets. The train set contains 80% of the data, while the test set contains the remaining 20%.

## Features
The input sequence length and the number of features are defined. In this case, the input sequence length is set to 7, and the number of features is equal to the number of columns in the data (in this case, 1).

## Input & Output
The input and output data for the LSTM model are created. The input data consists of sequences of length n_steps (7 in this case), and the output data is the next value in the sequence.

## Model
The LSTM model architecture is defined using the Sequential API from Keras. The model consists of two LSTM layers with dropout regularization and a fully connected layer. The model is compiled with the Adam optimizer and the mean squared error loss function.

The model is trained using the training data for a specified number of epochs.

## Prediction
The model is used to predict the stock price for a given number of days into the future. The last input sequence from the training data is used to initialize the prediction process. The model predicts the next day's value and appends it to the predicted values array. The process is repeated for the desired number of days.

The predicted values are unnormalized using the MinMaxScaler, and a line plot is created to visualize the predicted stock prices for the next days.

Please note that this project serves for educational purposes and should not be considered as financial advice.

Feel free to explore the provided code and modify it according to your requirements. Have fun experimenting with LSTM models for stock price prediction!
