
Tenacity Titans - H4FT 2024 - Business Case #1
Overview
This project, completed by Team Tenacity Titans for the H4FT 2024 challenge, focuses on analyzing and predicting stock price trends within the steel industry, specifically HPG Group stock. The project explores various statistical and machine learning models to gain insights into market trends, identify significant factors impacting stock prices, and develop accurate predictive models.

Table of Contents
Overview
Data Transformation
Exploratory Data Analysis
Feature Engineering
Modeling
ARIMA Model
LSTM Model
Model Comparison
Results
Conclusion
Requirements
How to Run
License
Data Transformation
Missing Values: Addressed missing values primarily due to market closures on weekends and holidays.
Data Types: Converted data types appropriately (e.g., Date to datetime, and price-related columns to float).
Data Integrity: Verified no duplicate dates in this time-series dataset, resulting in a dataset of 1,308 rows and 6 columns.
Exploratory Data Analysis
Analyzed market conditions, observing two price peaks and their alignment with industry growth in 2020-2021.
Examined patterns in Open Price, Relative Strength Index (RSI), and Moving Average (MA) to understand underlying market trends.
Applied Quarterly Comparison to detect significant variances in price and trading volume.
Feature Engineering
Selected Price as the primary feature for prediction based on its high correlation with other price-related variables and low correlation with volume, ensuring optimal model focus.

Modeling
ARIMA Model
Stationarity Check: Utilized the Dickey-Fuller test and differencing to achieve stationarity.
ACF & PACF Analysis: Guided ARIMA parameter selection through autocorrelation insights.
Model Selection: Identified an optimal ARIMA(2, 1, 0) model with the lowest AIC of -6116.61.
LSTM Model
Data Normalization: Normalized price data to enhance training performance.
Sequence Creation: Structured time series sequences for both training and testing.
Architecture: Built a deep learning model with two LSTM layers and Dense layers, trained for 1 epoch.
Model Comparison
Metric	ARIMA	LSTM
MAE	0.0243	1181.5377
RMSE	0.0326	1440.2883
R² Score	0.9638	0.7185
Results
The ARIMA model demonstrated superior accuracy and lower error magnitudes compared to the LSTM model, making it a more reliable choice for short-term forecasting in this dataset.

Conclusion
The ARIMA model provides an effective approach for short-term predictions, though further refinements are necessary for longer-term reliability. This analysis underscores the importance of using robust statistical methods for accurate stock price predictions in volatile markets.

Requirements