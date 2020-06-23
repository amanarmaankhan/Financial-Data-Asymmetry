# Financial-Data-Asymmetry
Architecture of Financial data asymmetry:
1.Many-to-One Sequence Problems with a Single Feature:
Here I have LSTM model for time series data forcasting and we have Data of a company with the stock prices of past 'Y' days closing,opening,high,low.
Firstly we have to make our data perfect,for that extract only the closing stock price coloumn and store in an array.
Split the data into train and test,let us take there are  'X' days of  closing stock price data.
Then as the input should be in 3D shape ,we reshape our data into [samples, time-steps, features] here as we have 1600 days of data which means 'X' samples and usually the time steps are taken in the range of 50-80 for few years of data.
The feature I have used is only one which is closing time.
Now this will create 










One-to-One Sequence with Multiple Features: As we have a sequence of data(sequence of closing stock price and opening price) as input and we have to predict a single output(closing stock price).
