1) Introduction

Retails stores like Walmart rely heavily on their inventory related supply chain logistics and is a key factor for them to make profit. The motivation of this work is to reduce the gap between supply and demand of goods sold by Walmart to customers all around the world.

This helps Walmart minimize inventory problems at these stores and also ensure customer satisfaction. Additionally, this helps Walmart reduce wastage, and save costs since mapping demand to supply would mean more products when demand is high and fewer products when demand is lower.

We intend to solve the problem by using machine learning models in the domain of regression. This machine learning model can be employed in various industries, in which demand and supply can be met at the same time.

3) Dataset

The dataset is walmart.csv from the website - https://www.kaggle.com/datasets/yasserh/walmart-dataset

4) Approach

We did an exploratory data analysis from which we got some interesting insights in the data-

Temperature influences weekly sales.The weeks having extremely high and low tempratures have less weekly sales
The holidays influence weekly sales. The holidays have higher average weekly sales
Another effect of holiday on sales. December has the highest average weekly sales. This is probably due to Christmas.
Feature selection and feature engineering

Implemented correlation matrix to find the relation between different factors.
Created a Baseline using mean as the baseline by implementing dummy regressor.

Implemented a Pipeline which used Robust Scaler and predicted the weekly sales using Temprature,Fuel Price,CPI ,Unemployment rate.
Calculated mean squared error for the baseline.
Implementing and Evaluating different ML models

The ML models were implemented using ML Pipeline and used RobustScaler.
To find the best hyper parameters for each ML model
Grid Search Cross Validation was used to find the best hyperparameters.
Negative Root Mean Squared Error was used as the evaluation measure.
The Best Model was selected

The Best Model was Gradient Boosting Regression because it has the least Negative Root Mean Squared Error.
The Best Hyper Parameters were also obtained.
The Best Model was tested on Testing data set to predict the weekly sales

The Mean squared error, Mean absolute error and R2 score were found out.
The Gradient Boosting Regressor has an R2 score of 0.96
