# Bitcoin-Closing-Price-Prediction
This project goal is to predicts the closing price of Bitcoin 7 days ahead from the last date of dataset using the Long Short Term Memory (LSTM) algorithm based on the supporting social sentiments using Valence Aware Dictionary for Sentiment Reasoning (VADER) model to analyzed social sentiment. Historical price of Bitcoin, Ethereum, and Litecoin, social sentiment data from Twitter and Google News used for this study as much as 152,592 data hourly basis from January 1, 2020 to July 31, 2021. The result of this research is to predict Bitcoin closing price with a calculation of error using Root Mean Squared Error (RMSE) metrics is 2731.99 and accuracy rate using Mean Absolute Percentage Error (MAPE) metrics with percentage of 95.22%.

# Data Collection
* Cryptocurrencies historical data obtained downloaded from https://cryptodatadownload.com/ sourced from Bitstamp Exchange Data platform with trade rate data 1 hour interval in USD exchange rates
* Social sentiment data from https://twitter.com obtain using web scrapping utilizing Twint API
* Social sentiment data from https://news.google.com using web crawling utilizing BeautifulSoap Library

# Data Preprocessing
  Preprocessing data including sentiment analysis process using Valence Aware Dictionary and Sentiment Reasoner (VADER) Model. Social sentiment data is trained for labelling. This stage performs the process of combining, normalizing, splitting data into training and testing set and determining the length of data input.

# Training and Testing Model
  The model is made by LSTM algorithm using Keras library in Python to train input data with several parameters like LSTM neurons, epochs, and batch size. At this stage determining training parameter is used to produce an optimal model for input data. Every model is evaluated for its performing using Root Mean Squared Error metrics and Mean Absolute Percentage Error metrics
 
 # Prediction
  Optimal model is used for predict Bitcoin price. Input data in form of normalization is denormalized to get prediction data. This study predicts 7 days prediction from August 1, 2021 until August 7, 2021.
  
  <p align="center">Visualization Test Results and Predictions</p>
  
![img](https://github.com/fajarhusain08/Bitcoin-Closing-Price-Prediction/blob/master/Prediction.PNG)
<p align="center">Comparison Plot Between Actual Price and Price Prediction</p>
