# Real Estate Analysis

## Overview

This project is an analysis of real estate within California. The goal of the project is to be able to predict sale price based on the features of the house. 

## Business Problem

The business problem for this project is to accurately price houses for sale according to the features of the house. Being able to accurately price houses lets people see the true value of a home and reference it against the listing price to save more money when shopping for their new home.

## Data

The [California Real Estate dataset from Kaggle](https://www.kaggle.com/datasets/yellowj4acket/real-estate-california) has around 35,000 records of houses within the state. There are a total of 38 columns and include data such as location, size, and amenities. Many of the feature variables included in the final analysis are important because they are features that impact the value of a home.

## Methods

By using Python and its packages such as numpy and pandas, we explored the data's features and their relationship to our target variable, popularity. After exploration, we used other libraries such as scikit-learn to model our predictions. Within scikit-learn, we iterated through linear regression and random forest regression models to predict popularity. The metric used to evaluate the models was the RMSE score. The R2 score was also observed.

## Results

Our evaluation metric in this project was mainly the RMSE score while also observing the r2 score. The RMSE score is a measure of the square root the mean squared error, which measures the average of the distances between the actual popularity and the predicted popularity. The goal for this project is to minimize that distance. The r2 score tells us what % of the variance is explained by the model and we try to get this value as high as possible. The RMSE scores for our linear regression models were almost the same, indicating that the training and test predictions performed roughly the same for each iteration. The decision tree model also performed roughly the same on the training and validation set and had the worst performance. The random forest regression model performed poorly on the validation set, indicating it was overfit. Although the models were overfit, they still performed better than our baseline model. 
