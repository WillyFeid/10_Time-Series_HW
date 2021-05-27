# 10_Time-Series_HW
Unit 10 - A Yen For The Future

# Overview
In this assignment we used time-series forecasting tools and linear regression modeling to predict future movements in the value of the Japenese yen versus the U.S. dollar.

## Technologies
I used a Hodrick-Prescott Filter to decompose the settle price into trend and noise. Then, I used ARMA to forecast Returns and an ARIMA model to forecast the settle price. I measured volatility with a GARCH model.
In the Linear Regression section, I split the data into training and testing data. From there, I fit a Linear Regression Model and made predictions using the testing data. I was then able to determine the performance of the out-of-sample and in-sample models by calculating the root mean square error.

## Findings
In the ARMA model, lags 4 and 5 were not a good fit (p>0.05), but this model suggests that retunrs will decrease over next 5-days. The ARIMA model also had high p values suggesting it's not a great fit. The ARIMA model suggests that the relative price of the Yen will increase over the next 5 days. The GARCH model was a great fit and shows a high level of forecasted volatility. 
Our Linear Regression model worked better with the out-of-sample data than it did with in-sample data, given the lower RMSE of the out-of-sample model performance.
