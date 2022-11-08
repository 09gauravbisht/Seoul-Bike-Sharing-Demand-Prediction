# Seoul-Bike-Sharing-Demand-Prediction

Problem Description:
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.


Data Description:
The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.
Attribute Information:
Date : year-month-day
Rented Bike count - Count of bikes rented at each hour
Hour - Hour of the day
Temperature-Temperature in Celsius
Humidity - %
Windspeed - m/s
Visibility - 10m
Dew point temperature - Celsius
Solar radiation - MJ/m2
Rainfall - mm
Snowfall - cm
Seasons - Winter, Spring, Summer, Autumn
Holiday - Holiday/No holiday
Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)

Project Description:
Bike sharing systems are a means of renting bicycles where the process of obtaining membership, rental, and bike return is automated throughout a city. Using these systems, people are able rent a bike from a one location and return it to a different place an there need.

Bike rental service scheme is a shared transport service in which bicycles are made available for shared use to individuals on a short-term basis for a price or free.

Predicting bike-sharing demand can help bike-sharing companies to allocate bikes better and ensure sufficient circulation of bikes for customers.

Steps Envolved:
1. Analyzing the problem: We will analyze the given dataset and find meaningful assumptions regarding the significance of this problem.

2. EDA / Preparing Data: While doing Exploratory Data Analysis, we will find meaningful information from the dataset.

3. Applying Models: We will use different regression models and find which model best fits our dataset to find the best prediction.

4. Feature Importance: We will also obtain which features will most likely affect the dependent variable (number of bikes rented) in each model.

Algorithms used:
1. Linear Regression

2. Random Forest

3. Gradient Boosting Machine

4. XGBoost

Best Hyper-parameters:
Random Forest:
max_depth : 8

min_samples_leaf : 40

min_samples_split : 50

n_estimators : 100

GBM:
max_depth : 8

min_samples_leaf : 40

min_samples_split : 50

n_estimators : 80

XGBoost:
eval_metric : rmse

max_depth : 6

n_estimators : 500


OBSERVATIONS:
* The feature variable Functioning Day has the highest impact on the dependent variable Rented Bike Count.
* In Random Forest and GBM, Temperature is making an impact while Rainfall is the second most important factor in XGBOOST.
* Random Forest & GBM gives importance to 6-7 features while XGBOOST considers only the top 3-4 features and almost neglects all the rest.
*
CONCLUSION:
* The project focuses on predicting bike sharing demand using the Seoul dataset.
* In this prediction we used different models and after getting the evaluation score we came to a conclusion that out of all the models used XGBOOST performs the best with the train R2 score of 0.96 & the test R2 of 0.87.
* XGboost gives the least MAE among the models. The most important features for predicting the dependent variable (number of hired bikes) for XGBoost are functioning day, rainfall, season, and temperature.
* This project will be helpful for the company to predict the hourly bike demand and enhance the user experience.
