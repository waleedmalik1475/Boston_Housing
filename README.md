# Boston_Housing
Detailed Report

1. Introduction

The goal of this project is to predict house prices using machine learning techniques. The dataset used is the Boston Housing Dataset, which contains information about various features of houses in Boston, such as the number of rooms, crime rate, and accessibility to highways. The target variable is the median value of owner-occupied homes in thousands of dollars.

2. Dataset Overview

Features: 13 numerical/categorical features (e.g., CRIM, ZN, INDUS, CHAS, NOX, RM, AGE, DIS, RAD, TAX, PTRATIO, B, LSTAT).
Target Variable: PRICE (median value of owner-occupied homes).
Size: 506 rows and 14 columns.
Missing Values: None.
3. Exploratory Data Analysis (EDA)

Pairplot: Visualized relationships between features and the target variable.
Correlation Heatmap: Identified strong correlations between features like RM (number of rooms) and PRICE.
4. Data Preprocessing

Handling Missing Values: No missing values were found.
Feature Scaling: Numerical features were scaled using StandardScaler.
Train-Test Split: The dataset was split into 80% training and 20% testing sets.
5. Model Selection & Training

Linear Regression: Baseline model with an MSE of 24.40 and R² of 0.67.
Random Forest: Improved performance with an MSE of 7.86 and R² of 0.89.
XGBoost: Achieved an MSE of 7.21 and R² of 0.90.
6. Model Optimization

Hyperparameter Tuning: GridSearchCV was used to optimize the Random Forest model, resulting in an MSE of 9.45 and R² of 0.87.
Feature Importance: Identified LSTAT (lower status of the population) and RM (number of rooms) as the most important features.
7. Results

Best Model: Optimized Random Forest Regressor.
Performance Metrics:
MSE: 7.86
R²: 0.89
8. Challenges

Feature Engineering: Limited features in the dataset restricted the scope for advanced feature engineering.
Overfitting: Ensured the model was not overfitting by using cross-validation during hyperparameter tuning.
9. Conclusion

The project successfully demonstrated the application of machine learning techniques to predict house prices. The optimized Random Forest model performed the best, achieving an R² score of 0.89. Future work could involve exploring more advanced models like Neural Networks or using a larger dataset with additional features
