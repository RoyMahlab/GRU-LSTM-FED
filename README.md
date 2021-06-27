# GRU-LSTM-FED - Description
Python implementation for NASDAQ-100 price prediction using FED's assets.
![image](https://user-images.githubusercontent.com/66019798/123539089-ac170280-d740-11eb-8720-c61655529faa.png)

# Reference
Based on the work "Predicting Stock Price using LSTM model, PyTorch" by Taron Zakaryan, Paris, Île-de-France, France.

Project site can be found here: https://www.kaggle.com/taronzakaryan/predicting-stock-price-using-lstm-model-pytorch

# Agenda
The Federal Reserve System (also known as the Federal Reserve or simply the Fed) is the central banking system of the United States of America.

Since the corona-virus pandemic broke, the United States Federal Reserve 
assets nearly doubled, which raised claims that the Fed is inflating the value of assets in the stock market.

In our project we will examine this claim. We will do so by implementing 2 different methods for RNN models, and compare their results with
each other and examine the influence of the FED's assets on the results.

We can divide the workflow into few main steps:

Loading the data

Spliting the data

Building the LSTM and GRU models

Using OPTUNA for tuning of hyper parameters

Compering the results and the naive prediction (average weekly gain)

Presenting the results
# Training methods
For our project's models we chose Adam (Adaptive Moment) as our optimizer, stepLRonPlateu as our scheduler and MSE as our loss function.

# Parameters
The hyper parameters we used OPTUNA to tune are:

Batch Size

Hidden Dim

Number of layers

Learning Rate

Number of Iterations

Factor

Look Back

Patience

# DATA Sources
Nasdaq 100-values:
https://finance.yahoo.com/quote/%5ENDX/history?period1=958608000&period2=1621296000&interval=1wk&filter=history&frequency=1wk&includeAdjustedClose=true

Fed total assets:
https://fred.stlouisfed.org/series/WALCL

