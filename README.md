# Retail Store Sales Forecasting

This repository details my work on ML Sales Forecasting, completed during my internship as a Machine Learning Engineer. The project involves applying advanced machine learning techniques to forecast sales, providing valuable business insights.

***

## Overview

### The Data Set
The forecasting model relies on the WOMart Data Set, available from Kaggle. For more details and to access the data, please visit [Kaggle's WOMart Data Set](https://www.kaggle.com/datasets/shelvigarg/sales-forecasting-womart-store).

### Objectives
- To develop a predictive model that can accurately forecast future sales.
- To implement various machine learning algorithms and compare their performance.
- To enhance decision-making and strategic planning for retail operations.

***

### Data Preparation & Feature Engineering

I streamlined the dataset and enhanced it with several engineered features to optimize the performance of our forecasting models. Including, 
- **Categorical variables** such as Store Type, Location Type, and Region Code
- **Lag Sales Values**: Utilized lagged sales values to capture temporal dependencies and trends.

***

### Models & Evaluation

Implemented multiple models and evaluated them to find the most effective approach:
- **Models Used**: Decision Tree, Random Forest, LightGBM, Elastic Net, KNN, Gradient Boost, CatBoost, XGBoost
- **Evaluation Metrics**: R² Score, MAE, MSE, RMSE, MAPE

***

### Model Selection and Iterative Process

- **Lag Features and Predictive Accuracy**: Initially, the models were assessed based on their ability to effectively utilize historical lagged values. This evaluation was essential for understanding how each model could predict future sales by analyzing past data trends.

- **Iterative Process Using Predicted Lags**: After the initial assessment, the process involved using the models to forecast new lag values, which were then used as inputs in a continuous feedback loop. This approach simulated real-time forecasting and provided deeper insights into each model's practical performance under conditions where direct historical data was not available.

This method led to the selection of **XGBoost** as the most effective model. It not only showed superior performance with historical data but also proved to be the most reliable when utilizing dynamically predicted lag values for forecasting future trends. The model's robustness in handling predicted lags solidified its practical applicability in real-world scenarios.


***

### Achievement 🏆
Achieved the highest R² Score and lowest error metrics across all models, setting a new standard of excellence in sales forecasting during my internship.
