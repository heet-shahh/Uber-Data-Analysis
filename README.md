# Uber Data Analysis

## Overview

Uber, a pioneering ride-sharing service, generates extensive data on rides and deliveries. This project focuses on developing an accurate price prediction model for Uber rides, taking into account various influential factors such as location, distance, time, weather, cab types, and more. Through Exploratory Data Analysis (EDA), we aim to uncover insights and visualize the relationships between these factors.

## Dataset

The dataset used for this project is sourced from Kaggle and can be accessed [here](https://www.kaggle.com/brllrb/uber-and-lyft-dataset-boston-ma). It spans two months of ride information in Boston, MA, with approximately 600,000 rows and 57 feature columns. The dataset covers essential ride attributes and detailed weather data, providing a comprehensive basis for analysis.

## Data Preparation

The initial stages involve meticulous data cleaning and transformation. We focus exclusively on Uber rides, filtering out other ride types to narrow our analysis. Notably, around 50,000 missing values for price are associated with Taxi rides. To ensure accuracy, consistency, and error-free data, we've dropped rows with missing values, which won't impact our analysis of Uber rides.

## Data Visualization

Data visualization plays a pivotal role in understanding the dataset. We've employed various visualization techniques, including barplots, scatterplots, and strip plots, to explore relationships such as hourly ride counts, rides based on weather forecasts, and price vs. distance.

## Machine Learning Models

Categorical values have been transformed using Label Encoder and fed as inputs to machine learning models. Four models were employed for price prediction: Linear Regression, Decision Tree Regressor, Random Forest Regressor, and XGBoost (Extreme Gradient Boost) Regressor. Scikit-learn library has been extensively utilized for model development.

## Model Evaluation

After fine-tuning the model parameters, XGBoost emerged as the top performer, achieving an impressive 95.4% accuracy on the test dataset. Random Forest also performed well but with a longer training time. We further analyzed feature importance and found that only five features had the most significant impact on prediction.

## Evaluation Metrics

The following evaluation metrics were obtained for the XGBoost predictions on the test data:

- Mean Absolute Error (MAE): 1.12
- Mean Squared Error (MSE): 3.31
- Root Mean Absolute Error (RMAE): 1.82

## Regression Plots

Regression plots for Random Forest and XGBoost predictions:
![Random Forest](https://github.com/heet-shahh/Uber-Data-Analysis/assets/141808272/c0cb0341-3747-46f9-9620-c0d37770e23e)
![XGBoost](https://github.com/heet-shahh/Uber-Data-Analysis/assets/141808272/58d4eb45-5989-4c1f-b6c7-d4e73e464ad0)

## Conclusion

This project encompasses a comprehensive journey through the data analysis process. From data preparation to visualization and predictive analysis, it offers detailed explanations, code snippets, and visualizations to illuminate the results. Through exploring Uber's dataset, we've gained valuable insights into the factors influencing ride prices, ultimately developing an accurate pricing model.
