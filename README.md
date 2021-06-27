# GRU-LSTM-FED
Python implementation NASDAQ-100 price prediction using FED's assets 
Based on the work "Predicting Stock Price using LSTM model, PyTorch" by Taron Zakaryan, Paris, Île-de-France, France
Project site can be found here: https://www.kaggle.com/taronzakaryan/predicting-stock-price-using-lstm-model-pytorch

The Federal Reserve System (also known as the Federal Reserve or simply the Fed) is the central banking system of the United States of America.

Since the corona-virus pandemic broke, the United States Federal Reserve 
assets nearly doubled, which raised claims that the Fed is inflating the value of assets in the stock market.

In our project we will examine this claim. We will do so by implementing 2 different methods for RNN models, and compare their results with
each other and examine the influence of the FED's assets on the results.

We can divide the workflow into few main steps:

Loading the data.
Spliting the data.
Building the LSTM and GRU models.
Using OPTUNA for tuning of hyper parameters.
Compering the results with themselves and with the naive prediction (average weekly gain).
Presenting the results.

# Parameters
Batch Size
Hidden Dim
N layers
Learning Rate
Num Iters
Factor
Look Back
Patience 
# Folders

# Reference
