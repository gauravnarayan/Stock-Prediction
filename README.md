# GE Stock price prediction

Downloaded 5 years of daily stock prices from Yahoo Finance. The data has Date, Open, High, Low, Close, Adj Close, and Volume for each day. 
Considered only Open, High, Low, and Close for the model. 

Used a ‘lazy window’ of size 20 to predict the 21st stock price value using an LSTM. 
To do this, flatten the stock data first. Then re-shape this one-dimensional array into a tensor of shape (?, 20, 1).
Get every 21st stock price and put it into the target. 
Used train: test split ratio of 75:25. 
Created a plot of predicted stock prices and actual stock prices.

Used a proper window of size 20 to predict the next stock price value using an LSTM.
To do this, flatten the stock data first. Then re-shape this one-dimensional array into a tensor of shape (?, 20, 1).
Got every stock price (21st,22nd,23rd....5000..) and put it into the target. 
Used train: test split ratio of 75:25. 
Created a plot of predicted stock prices and actual stock prices.
