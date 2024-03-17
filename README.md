# GE Stock price prediction

Downloaded 5 years of daily stock prices from Yahoo Finance. The data has Date,Open, High, Low, Close, Adj Close and Volume for each day. 
Considering only Open, High, Low, and Close for the model. 

Using a ‘lazy window’ of size 20 to predict the 21st stock price value using an LSTM. 
To do this, flattened the stock data first. Then re-shape this one-dimensional array into a tensor of shape (?, 20, 1).
Got every 21st stock price and put it into the target. 
Used train:test split ratio of 75:25. 
Created a plot of predicted stock prices and actual stock prices.

Using a proper window of size 20 to predict the next stock price value using an LSTM.
To do this, flattened the stock data first. Then re-shape this one-dimensional array into a tensor of shape (?, 20, 1).
Got every stock price (21st,22nd,23rd....5016) and put it into the target. 
Used train:test split ratio of 75:25. 
Created a plot of predicted stock prices and actual stock prices.
