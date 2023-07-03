# Stock Sentiment Analysis - Google News & Twitter
This code provides functionality to analyze the sentiment of news articles and tweets related to a specific stock ticker. It utilizes the News API to retrieve news articles and the Twitter API to fetch tweets for sentiment analysis. The sentiment analysis is performed using the TextBlob library, and the results are visualized using matplotlib.

## Prerequisites
Before running the code, ensure you have the following:

Python 3 installed
Required libraries: requests, tweepy, textblob, matplotlib, numpy

## Getting Started
Clone the repository or copy the code into your local environment.

Install the required libraries using pip:
pip install requests tweepy textblob matplotlib numpy

Obtain API keys:

For the News API, visit https://newsapi.org/ and sign up for an API key.
For the Twitter API, create a Twitter Developer account at https://developer.twitter.com/. Create a new app and generate the required access tokens.

## Usage
### Sentiment Analysis of News Articles
Provide your News API key when prompted.

Run the code and enter the stock ticker you want to analyze.

The code will retrieve news articles related to the provided stock ticker using the News API. It will then analyze the sentiment of each article's title and display the sentiment distribution as a pie chart.

### Sentiment Analysis of Tweets
Provide your Twitter API credentials (consumer key, consumer secret, access token, and access token secret) when prompted.

Run the code and enter the stock ticker you want to analyze.

The code will authenticate with the Twitter API using the provided credentials. It will then fetch a specified number of tweets containing the stock ticker and perform sentiment analysis on the text of each tweet. The sentiment distribution will be displayed as a pie chart.

## Results
The sentiment analysis results will be printed to the console, showing the total count and percentage of positive, neutral, and negative articles/tweets. Additionally, a pie chart will be displayed to visualize the sentiment distribution.

Please note that the sentiment analysis is based on the polarity of the text and may not always accurately reflect the true sentiment. Use the results as a general indication and exercise caution in making financial decisions based on sentiment analysis alone.

## Troubleshooting
If you encounter any issues or errors while running the code, please ensure that you have correctly installed the required libraries and provided valid API keys for the News API and Twitter API.

For further assistance, please refer to the official documentation of the respective APIs:

News API: https://newsapi.org/docs
Twitter API: https://developer.twitter.com/en/docs

## License
This project is licensed under the MIT License. Feel free to modify and use the code as per your requirements.

## Acknowledgments
News API - Provides access to a wide range of news articles.
Tweepy - Python library for accessing the Twitter API.
TextBlob - Python library for natural language processing and sentiment analysis.
Matplotlib - Library for creating visualizations in Python.
NumPy - Library for numerical computations in Python.

## Disclaimer
This code is intended for educational and research purposes only. The sentiment analysis results should not be considered as financial advice. Always perform thorough analysis and consult with financial professionals before making any investment decisions.
