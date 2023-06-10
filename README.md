# XGBoost-model-applied-to-CBOT-Soybean-oil-closing-prices
CBOT Soybean oil closing price prediction using an XGBoost ML model applied to the 2014-2016 period.  
This the El Niño weather period. This model aims specifically at the soybean oil price performance &amp; its forecasting vs the exchange listed contracts used hedging risk strategies &amp; speculative bets traded at CBOT. 

This period is relevant as the El Niño weather event had a global reach with below or above-average rainfall & flooding impacting agricultural commodities as oilseeds, soft, grains, live stock & dairy products.
 
The model is interesting & a basic reference given the current El Nino weather impact is rising to a moderate level by Q4 2023/ Q1 2024.
Hence a weather market risk & hedging considerations applied.

**More technically**

The XGBoost model is a machine learning algorithm that is widely used for both supervised classification and regression problems. 
It provides a wrapper class to allow models to be treated like classifiers or regressors in the scikit-learn framework. 
This XGBoost model is trained using the XGBRegressor class, which is a regression model. 
The objective of the XGBoost model is to minimize the mean squared error between the predicted and actual closing prices. 
The XGBoost model is a flexible and powerful algorithm that can handle a variety of data types, relationships, and distributions. 
It provides a large number of hyperparameters that can be tuned to improve model performance.

In this code, we import the necessary libraries (pandas, numpy, xgboost, joblib, matplotlib.pyplot, tensorflow, tensorflow.keras, train_test_split) and retrieve CBOT soybean oil historical data for 2014-2016 from Quandl. 
We prepare the data by selecting the 'Settle' prices, creating features and labels, and standardizing the data. We then split the data into training and testing sets using the train_test_split function.

Next, we train an XGBoost model using TensorFlow's xgb.XGBRegressor class. The model is trained on the training data and tested on the testing data, with predictions stored in the y_pred variable.

The trained model is saved using the joblib.dump function with the specified filename. Finally, the performance of the model is visualized using a line plot, showing the predicted and actual closing prices.

Way to go but an interesting start & a great experience for me.
