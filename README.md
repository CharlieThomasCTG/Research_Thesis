# Stock Price Prediction using LSTM

# ![image](https://github.com/charliethomasct82/Research_Thesis/assets/93368865/fc8043a8-809e-45c7-bb00-482527850239)

# ![image](https://github.com/charliethomasct82/Research_Thesis/assets/93368865/bba15e9e-fd51-48e7-ae33-b62f59cf3c37)


# ![image](https://github.com/charliethomasct82/Research_Thesis/assets/93368865/6d5ad349-3583-48d3-9597-1f436de993d1)



# PROBLEM STATEMENT
Yes Bank was incorporated in the year 1999 by Ashok Kapur, Harkirat Singh and Rana Kapoor. Yes Bank’s Non-banking financial business has a shareholding pattern of 25 % of the business with former named incorporators and 75 % held by Rabo Bank from the Netherlands. Yes Bank Ltd. was listed on the BSE, Bombay Stock Exchange in May 2005 and also had a follow-up public offering in July 2020. The Bank faced a steep fall in stock price from mid-2019 because of mismanagement of loan lending, governance issues, false Assurance and lack of insight by the management. The Yes Bank collapsed financially and the government and other banks restructured the Yes Bank and helped it revamp its operation in 2019-20. Yes Bank Ltd. has fallen from an all-time high to an all-time in the last 5 years. This led to an influx of retail and corporate investors hoarding the shares of the bank. The turnaround of the bank, traders and investors' anticipation about the stock price and the high volume of the stock’s trade on the stock exchange motivated this study to develop an LSTM model that can predict the stock price of Yes Bank.
The research aims to compare the different forms of LSTM architectures such as Single-layer LSTM, bi-directional LSTM, and Multi-layer LSTM to predict the future price of Yes Bank Ltd. The study will utilize Yes Bank Ltd. Historical price data. Yes Bank has been one of the most traded stocks on the NSE and BSE, the stock exchange of  India. Investors(retail and corporate) have shown keen interest in the stock for long-term as well as short-term investments. The research aims to propose a model that would be able to predict the future price as well as trend in the moment of the stock. The research proposes to develop an LSTM model that will be less complex and would require historical price data to predict the future price of the stock.
1.3	OBJECTIVES AND AIM
The aim of this study is to propose an effective LSTM model that can provide stock price prediction with low variability. This will be achieved by comparing the performance of various LSTM architectures such as Single-layer LSTM, bi-directional LSTM, and Multi-layer LSTM to predict the future price of Yes Bank Ltd. To accomplish this, the research will incorporate predictors such as the daily historical prices such as Open price, Close price, High price and Low price on the given day. The research proposes to develop an LSTM model that will be less complex and would require historical price data to predict the future price of the stock. The research objectives are as follows: 
1.	The examination of patterns among various predictors, which comprises historical fundamental indicators like historical prices (open, high, low, close).
2.	A thorough comparison of the performance of various predictive models such as single-layer LSTM, bi-directional LSTM, and multi-layer LSTM.
3.	To run the trial for hyperparameter tuning to improve the performance of the model.
4.	To predict the trend of the stock.
   
# FlOW OF THE STUDY
![image](https://github.com/charliethomasct82/Research_Thesis/assets/93368865/970ab2f7-d8b6-44d1-a50b-2ba64949427e)

# RESEARCH QUESTIONS / HYPOTHESIS TESTING
The study used the Dickey-Fuller Test to check the stationary nature of the data. The test statistic used in the augmented Dickey-Fuller statistic is a negative number. The higher the negative number, the stronger the rejection of the hypothesis that there is a unit root at some level of confidence.

# HYPOTHESIS TESTING(Research Question 1)
Is the data stationary or non-stationary?
The following are the test hypotheses:
Null hypothesis (H0): The time series data is non-stationary. 
Alternate hypothesis (H1): The time series is stationary (or trend-stationary).

First, in the below plot 4.4.1.1, the rolling mean is increasing but the standard deviation is more or less constant. The test Statistics of -1.519420  is greater than the critical value at 1%,5% and 10%(refer to table 4.4.1.1). Therefore, It cannot be assumed with any confidence that this is a stationary series Moreover,  the p-value is higher than the 1%,5% and 10% threshold(refer to table 4.4.1.1). Hence the null hypothesis cannot be rejected at any confidence level. Meaning that the Dickey-Fuller test verifies that the time series is non-stationary.
# ![image](https://github.com/charliethomasct82/Research_Thesis/assets/93368865/c7594d17-68e6-4d0f-b8ff-1c1426caefc6)


We applied the log transformation and then we applied the square root transformation to make the data stationary. Then, we conducted the dickey-fuller test to check whether the non-stationary data changed to stationary data.

# HYPOTHESIS TESTING(Research Question 2)
Did the transformation of the data change the nature of the data to stationary?
The following are the test hypotheses:

Null hypothesis (H0): The applied transformation technique on time series data did not change the characteristics to stationary. 

Alternate hypothesis (H1): The applied transformation technique on time series data changed the characteristics of stationery.

First, in the below plot 4.4.1.1, the rolling mean and standard deviation are more or less consistent with each other’s movement over the period. The test statistic of -1.655430e+01 is a lot lower than the critical value at 1%,5%, and 10%(refer to Table 4.4.1.2). Therefore, It can be assumed with more than 99% confidence that this is a stationary series. Moreover,  the p-value is smaller than the 1%,5% and 10% threshold, thus the null hypothesis is rejected, meaning that the Dickey-Fuller test verifies that the time series is stationary.
#![image](https://github.com/charliethomasct82/Research_Thesis/assets/93368865/d8474cdc-59ba-4e31-a70d-cb18488a4570)
 



# STUDY'S SCOPE
The analysis of Yes Bank Ltd.'s stock examined its historical prices such as Open, Close, High, and low to propose an LSTM model that can predict the stock price. The study solely relied on Historical price information and information such as technical indicators, macroeconomic data, market sentiments etc. has not been incorporated. The study did not compare other machine learning algorithms and statistical models but three LSTM algorithms such as single-layer LSTM, multi-layer LSTM and Bi-directional LSTM.


# Proposed Model: Bi-directional LSTM Model
![image](https://github.com/charliethomasct82/Research_Thesis/assets/93368865/08bb3863-31e5-4563-b90a-27a8453c8b69)



# DISCUSSION AND CONCLUSION
Yesbank’s historical price data were retrieved from Yahoo finance data using the yfinance library in Python. The initial Features utilised for the rudimentary stage of analysis were the Close price, Open price, High price and Low price of the Yes bank for the period from 2005-05-12 to 2023-08-09.

Pandas profiling library was utilized to conduct univariate, bi-variate analysis. Uni-variate analysis established a linear upward trend till 2018 and then there was a price crash till mid-2020. Since mid-2020, the price has been experiencing a sideways movement as discussed in section 4.2.1. Bi-variate analysis finds an existence of high co-relation among the features. The stock's closing price was selected as a feature to be incorporated into the study because of the high correlation among the features. 
Hypothesis testing was done on the Yes bank stock price data set to determine if the data was stationary or non-stationary. The Dickey-Fuller test was used as a statistical tool to perform hypothesis testing. The test established that data is non-stationary with more than 99% confidence. Log transformation and then square transformation were performed to flatten it. Dicky-fuller test confirmed that transformed data is stationary with more than 99% confidence. An intuitive method was implemented to create a new data set from transformed data. The previous three days' close prices were used to predict the close price of the next day. The previous three day’s price was used as the explanatory variable and every 4th-day’s price was treated as the predictor variable. 80% per cent of the data was kept as Training data and 20% of the data was treated as test data. 30% of the data in the training dataset was treated as Validation data. Training and test data were converted into a NumPy array to feed into the LSTM model.

Initially, three baseline models were built, namely single-layer LSTM, multi-layer LSTM and bi-directional LSTM. All three models were built with a number of RNN units=128, Adam as optimizer with a learning rate of 0.004.15 experiments were conducted on each baseline model. Hence total of 45 experiments were conducted. One best model was selected from the experiments conducted on three baseline models with different combinations of the number of epochs[10,20,50,100] and batch size[32,64,128,256]. Loss scores on the validation dataset of the baseline model and selected Experimental model were compared. 

An experimental Bi-directional model with epochs:10 and batch size: 64 was selected for hyperparameter tunning because it has the lowest Loss scores on the validation dataset of 322.02. Hyperparameter tuning has improved the Loss by 88.28% from 322.02 to 37.88 (refer to Plot 4.9.1). Hence, a Bi-directional tuned Model was implemented on the test data set. Hyperparameters of the proposed model are as follows: Epochs:10, batch size:64, Dropout rate: 0.4, learning rate: 0.0013489304109835225, Number of layers:12. Input units are the number of RNN units in each layer. input_unit1: 80, input_unit2: 32, input_unit3: 16, input_unit4: 16, input_unit5: 16, input_unit6: 16, input_unit7: 16, input_unit8: 16, input_unit9: 16, input_unit10: 16, input_unit11: 16, input_unit12: 16(refer to Table 4.8.1, trial 1). Adam optimizer was selected based on understanding from the literature review.  The proposed model predicted the stock price very close to actual values with Loss and RMSE scores of 25.004 and 5.02, and also captured the moment of the stock very well as discussed in Chapter 5, Results.

The proposed model was implemented on the unseen test data containing Yes Bank’s share price for the period from 03-01-2020 to 04-08-2023. The proposed model was able to predict the price with a loss Score of 25.024.
                                                           


