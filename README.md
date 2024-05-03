# Stock Price Prediction using LSTM
#![image](https://github.com/charliethomasct82/Research_Thesis/assets/93368865/3ba2b736-a9c2-4977-a4ca-8be3283f4aa2)



# PROBLEM STATEMENT
Yes Bank was incorporated in the year 1999 by Ashok Kapur, Harkirat Singh and Rana Kapoor. Yes Bank’s Non-banking financial business has a shareholding pattern of 25 % of the business with former named incorporators and 75 % held by Rabo Bank from the Netherlands. Yes Bank Ltd. was listed on the BSE, Bombay Stock Exchange in May 2005 and also had a follow-up public offering in July 2020. The Bank faced a steep fall in stock price from mid-2019 because of mismanagement of loan lending, governance issues, false Assurance and lack of insight by the management. The Yes Bank collapsed financially and the government and other banks restructured the Yes Bank and helped it revamp its operation in 2019-20. Yes Bank Ltd. has fallen from an all-time high to an all-time in the last 5 years. This led to an influx of retail and corporate investors hoarding the shares of the bank. The turnaround of the bank, traders and investors' anticipation about the stock price and the high volume of the stock’s trade on the stock exchange motivated this study to develop an LSTM model that can predict the stock price of Yes Bank.
The research aims to compare the different forms of LSTM architectures such as Single-layer LSTM, bi-directional LSTM, and Multi-layer LSTM to predict the future price of Yes Bank Ltd. The study will utilize Yes Bank Ltd. Historical price data. Yes Bank has been one of the most traded stocks on the NSE and BSE, the stock exchange of  India. Investors(retail and corporate) have shown keen interest in the stock for long-term as well as short-term investments. The research aims to propose a model that would be able to predict the future price as well as trend in the moment of the stock. The research proposes to develop an LSTM model that will be less complex and would require historical price data to predict the future price of the stock.
1.3	OBJECTIVES AND AIM
The aim of this study is to propose an effective LSTM model that can provide stock price prediction with low variability. This will be achieved by comparing the performance of various LSTM architectures such as Single-layer LSTM, bi-directional LSTM, and Multi-layer LSTM to predict the future price of Yes Bank Ltd. To accomplish this, the research will incorporate predictors such as the daily historical prices such as Open price, Close price, High price and Low price on the given day. The research proposes to develop an LSTM model that will be less complex and would require historical price data to predict the future price of the stock. The research objectives are as follows: 
1.	The examination of patterns among various predictors, which comprises historical fundamental indicators like historical prices (open, high, low, close).
2.	A thorough comparison of the performance of various predictive models such as single-layer LSTM, bi-directional LSTM, and multi-layer LSTM.
3.	To run the trial for hyperparameter tuning to improve the performance of the model.
4.	To predict the trend of the stock.
   
# RESEARCH QUESTIONS
1.	Is the data stationary or non-stationary?

The following are the test hypotheses:

Null hypothesis (H0): The time series data is non-stationary. 

Alternate hypothesis (H1): The time series is stationary (or trend-stationary).

2.	Did the Transformation of the data change the nature of the data to stationary?

The following are the test hypotheses:

Null hypothesis (H0): The applied transformation technique on time series data did not change the characteristics to stationary. 

Alternate hypothesis (H1): The Applied transformation technique on time series data changed the characteristics to stationary.  (or trend-stationary).

Research question 1 and 2 answered in section 4.4, Hypothesis testing

3.	Was the proposed model able to predict the trend of the stock on unseen data?
Research Question is Answered in Section 5.5 and  Plot 5.5.1

# STUDY'S SCOPE
The analysis of Yes Bank Ltd.'s stock examined its historical prices such as Open, Close, High, and low to propose an LSTM model that can predict the stock price. The study solely relied on Historical price information and information such as technical indicators, macroeconomic data, market sentiments etc. has not been incorporated. The study did not compare other machine learning algorithms and statistical models but three LSTM algorithms such as single-layer LSTM, multi-layer LSTM and Bi-directional LSTM.
