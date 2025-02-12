# Car-Price-Prediction-Model---Machine-Learning-End-Project
### Overview

This project aims to develop a machine learning model that can predict the price of cars based on various features such as car dimensions, engine specifications, fuel type, and more. The dataset is gathered from the American automobile market and serves as the foundation for understanding the key factors affecting car prices. By building different regression models, we identify the most significant variables impacting car prices and assess the performance of each model.
### Problem Description

A Chinese automobile company is looking to enter the US market by setting up a manufacturing unit and producing cars locally. To better understand how car pricing works in the American market, they contracted an automobile consulting company. The task is to determine which variables significantly affect the pricing of cars and build a model that can predict the price based on these factors.
### Dataset

The dataset used for this project contains various features of cars, including:
     - **Car dimensions (e.g., wheelbase, car length, car width)
     - **Engine specifications (e.g., horsepower, engine size, cylinder number)
     - **Fuel and drive types (e.g., fuel type, engine location, aspiration)
     - **Price (target variable)

You can access the dataset from the following link:
Car Price Dataset
### Business Goal

The goal of this project is to build a model that predicts car prices based on independent variables such as car specifications, engine details, and more. This will help the automobile company understand how different features affect car pricing and make informed decisions about car design and marketing strategies.
Steps Implemented
## 1. Data Loading and Preprocessing

 - **Loaded the dataset and performed initial data inspection.**
 - **Removed unnecessary columns (e.g., car_ID and CarName).**
 - **Encoded categorical features (e.g., fuel type, aspiration) using one-hot encoding.**
 - **Split the data into training and testing sets (80-20 split).**

## 2. Model Implementation

We implemented five different regression models to predict car prices:

 - **Linear Regression**
 - **Decision Tree Regressor**
 - **Random Forest Regressor**
 - **Gradient Boosting Regressor**
 - **Support Vector Regressor**

Each model was trained on the training set and evaluated based on R-squared, Mean Squared Error (MSE), and Mean Absolute Error (MAE).
## 3. Model Evaluation

 - **We compared the performance of each model using metrics like R-squared, MSE, and MAE.**
 - **Random Forest Regressor showed the best performance with an R-squared value of 0.95, followed by Gradient Boosting Regressor.**

## 4. Feature Importance Analysis

 - **We used the Random Forest model to identify the most significant features affecting car prices.**
 - **The top features included enginesize, curbweight, and highwaympg, among others.**
 - **Feature selection led to better model performance by reducing the number of features and focusing on the most impactful ones.**

## 5. Hyperparameter Tuning

 - **Hyperparameter tuning was performed using GridSearchCV to find the best parameters for the Random Forest model.**
 - **After tuning, we found the optimal parameters that improved the model's performance slightly.**

## 6. Model Deployment

 - **The best model, after hyperparameter tuning, was deployed to predict car prices.**
 - **A plot was created comparing actual vs predicted car prices to visualize the model's performance.**

### Performance Metrics

| Model               | R²    | MSE          | MAE     |
|---------------------|-------|--------------|---------|
| Random Forest       | 0.95  | 3.57e+06     | 1303.54 |
| Gradient Boosting   | 0.92  | 6.03e+06     | 1725.62 |
| Decision Tree       | 0.91  | 7.41e+06     | 1836.14 |
| Linear Regression   | 0.89  | 8.48e+06     | 2089.38 |
| Support Vector      | -0.10 | 8.70e+07     | 5707.11 |
### Top 10 Most Important Features

 - **enginesize: 57.93%**
 - **curbweight: 27.38%**
 - **highwaympg: 4.20%**
 - **horsepower: 2.61%**
 - **carwidth: 1.31%**
 - **carlength: 1.01%**
 - **wheelbase: 0.79%**
 - **peakrpm: 0.69%**
 - **citympg: 0.66%**
 - **boreratio: 0.53%**

## Conclusion

This project provides valuable insights into how different features affect the price of cars in the American market. The Random Forest model performed the best in terms of prediction accuracy. This model can be used by the consulting company to make informed decisions regarding pricing, design, and marketing strategies for the Chinese automobile company looking to enter the US market.
## Acknowledgements

 - **Dataset source: Car Price Dataset on Google Drive**
 - **Libraries used: Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn**
