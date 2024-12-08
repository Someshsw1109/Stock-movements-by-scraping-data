# Stock Sentiment Analysis and Price Prediction

This project combines sentiment analysis of Twitter data with stock price prediction using machine learning models like Random Forest and Support Vector Regression (SVR). The goal is to analyze public sentiment from Twitter, predict stock prices, and visualize the results.

## Features

- Fetch stock data using Yahoo Finance.
- Fetch and process tweets related to stock symbols.
- Perform sentiment analysis on the tweets.
- Predict stock prices using machine learning models.
- Visualize results through various plots.

## Requirements

Before running the project, ensure you have the following Python libraries installed:

```bash
!pip install yfinance
!pip install tweepy
!pip install nltk
!pip install scikit-learn
!pip install matplotlib
!pip install treeinterpreter
!pip install vaderSentiment
```

## Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/praneethapedapudi/stock-movement-analysis-based-on-twitter-data-capx-assignment.git
   cd stock-movement-analysis-based-on-twitter-data-capx-assignment
   ```

2. Install the required dependencies:

   ```bash
   !pip install -r requirements.txt
   ```

3. Make sure you have the necessary API credentials for **Tweepy** (Twitter API) and configure them in the code.

## Files

1. `main.py`: Main script that performs stock data fetching, tweet fetching, sentiment analysis, and price prediction.
2. `fetchTweets.py`: Script to fetch tweets using the Twitter API and store them in a CSV file.
3. `sentimentAnalysis.py`: Script to perform sentiment analysis on tweets using NLTK's VADER Sentiment Analyzer.
4. `stockData_{stockname}.csv`: Stock data CSV file fetched using Yahoo Finance.
5. `tweets_{stockname}.csv`: CSV file containing tweets related to a specific stock.
6. `processedTweets_{stockname}.csv`: Processed tweet data merged with stock data.
7. `sentimentAnalysis_{stockname}.csv`: Sentiment analysis results for the tweets.

## How to Run

1. **Fetch tweets**: Use the `fetchTweets` function to collect tweets related to a specific stock symbol and save them in a CSV file.

2. **Process tweets**: The `processTweets` function will combine tweet data and stock data, and save the processed data for further analysis.

3. **Run sentiment analysis**: The `sentimentAnalysis` function will analyze the sentiment of tweets using VADER.

4. **Train models and predict stock prices**: Use the `RandomForestModel` and `SVRModel` functions to train machine learning models and predict stock prices.

5. **Visualize results**: The `main()` function will display graphs and plots comparing predicted and actual stock prices.


Follow the prompts to input the stock symbol and date range.

## License

This project is open source and available under the [MIT License](LICENSE).

---
