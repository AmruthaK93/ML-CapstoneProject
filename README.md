# Car Price Prediction Project

## Problem Description
A Chinese automobile company is planning to enter the US market. They want to understand the pricing dynamics of cars in the US so they can effectively price their own cars. The company has collected a dataset containing various characteristics of cars and their corresponding prices.

## Business Goal
Build a predictive model to estimate the price of a car based on its features. Additionally, identify key variables that significantly influence car prices to help the company with market positioning and pricing strategy.

## Dataset
The dataset (`CarPrice_Assignment.csv`) contains 26 variables related to car attributes like engine size, horsepower, car width, and more, including the target variable: `price`.

## Key Components to be Fulfilled
1. Loading and Preprocessing
2. Model Implementation
3. Model Evaluation
4. Feature Importance Analysis
5. Hyperparameter Tuning

---

## 1. Loading and Preprocessing
- Imported essential libraries like Pandas, NumPy, Seaborn, and Scikit-learn.
- Loaded and explored the dataset.
- Checked for null values and data types.
- Extracted car company names from the `CarName` field.
- Fixed inconsistencies in company names (e.g., correcting typos).
- Converted categorical features using one-hot encoding.
- Dropped irrelevant columns like `car_ID` and original `CarName`.

## 2. Model Implementation
### 2.1 Linear Regression
- Applied linear regression model.
- Interpreted coefficients to understand variable relationships.

### 2.2 Decision Tree Regressor
- Implemented a decision tree for non-linear modeling.
- Tuned `max_depth` and `min_samples_split`.

### 2.3 Random Forest Regressor
- Ensemble model that reduced overfitting.
- Feature importances were visualized and interpreted.

### 2.4 Gradient Boosting Regressor
- Implemented gradient boosting for improved accuracy.
- Performed better than Random Forest in some metrics.

### 2.5 Support Vector Regressor
- Applied SVR with feature scaling.
- Experimented with different kernels.

## 3. Model Evaluation
- Evaluated all models using metrics:
  - R-squared
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
- Random Forest and Gradient Boosting yielded the best performance.

## 4. Feature Importance Analysis
- Identified key predictors:
  - `engine size`
  - `curb weight`
  - `horsepower`
  - `car width`
  - `highway mpg`
- Visualized using bar plots.

## 5. Hyperparameter Tuning
- Used GridSearchCV for tuning models like Random Forest and SVR.
- Optimal parameters led to improved accuracy and generalization.

---

## Conclusion
- Engine size and curb weight are the most influential factors in determining car price.
- Ensemble methods like Random Forest and Gradient Boosting outperform simpler models.
- A robust predictive model was built and evaluated.
- These insights can help the company strategically price their cars in the US market.

---

## Future Scope
- Deploy model with a user-friendly dashboard.
- Explore deep learning models for improved performance.
- Use real-time data for dynamic pricing strategies.

---


This project was built as part of the Machine Learning module.

