# Stock_Price_Prediction

# Data
I have used the Netflix stock prices for the task. The data includes columns for date, high, low, open, close, volume, and adjusted close. I have focused on the "close" column for our prediction.

# Data Preparation
Initialize a variable called "sequence length" to determine the length of each sequence. Each sequence will consist of the first "sequence length" elements from the "close" column. The target for each sequence will be the next day's stock price. Created multiple samples by shifting the sequence one step to the right.

# LSTM Approach
Used an LSTM neural network for the prediction. Each element in a sequence will be fed into the LSTM.   The hidden state and cell state will be passed to the next LSTM. The output of the last LSTM cell will be fed into a feed-forward neural network to predict the next day's stock price.

# Implementation
Import the necessary libraries: numpy, pandas, sklearn, and matplotlib. Load the dataframe using pd.read_csv and print the head of the dataframe. Extract the "close" prices from the dataframe.

