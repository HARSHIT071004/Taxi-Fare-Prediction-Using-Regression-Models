Fare Prediction Using Machine Learning
Project Overview

This project focuses on predicting taxi fares using various regression techniques. The goal is to estimate fare amounts based on trip and temporal features while optimizing performance using feature engineering, model tuning, and evaluation. Multiple models were explored including Linear Regression, Polynomial Regression, Decision Tree, and Random Forest Regressors.

Key Features

Data Preprocessing & Feature Engineering:

Extracted temporal features (hour, day, month, year, day of week)

Handled missing values and scaling of numerical features

Calculated trip distance and considered passenger count as predictors

Regression Models Implemented:

Linear Regression: Standard baseline model

Polynomial Regression (degree=2): Captures non-linear relationships

Decision Tree Regressor: Handles non-linear patterns with max depth control

Random Forest Regressor: Ensemble method for improved accuracy

GridSearchCV: Hyperparameter tuning for Random Forest

Evaluation Metrics:

R² Score: Measures variance explained by the model

RMSE: Measures prediction error magnitude

Model Performance Summary
Model	R² Score	RMSE
Linear Regression	0.7142	2.9117
Polynomial Regression (deg=2)	0.7263	2.8493
Decision Tree Regressor	0.7638	2.6473
Random Forest Regressor	0.7769	2.5725

Conclusion: Random Forest Regressor provided the best performance.

Key Insights

Trip distance is the strongest predictor of fare.

Time-based features (hour, day of week) and passenger count significantly influence fare.

Feature scaling improves performance for models like SVR (commented due to computation time).

Hyperparameter tuning via GridSearchCV enhanced Random Forest performance.

Tech Stack

Python 3.x

pandas, numpy

scikit-learn

matplotlib, seaborn

How to Use

Load the dataset and clean it.

Perform EDA to understand feature distributions and correlations.

Split the data into training and testing sets.

Scale features where required.

Train regression models (Linear, Polynomial, Decision Tree, Random Forest).

Tune hyperparameters for Random Forest using GridSearchCV.

Evaluate models with R² and RMSE metrics.

Future Work

Experiment with Gradient Boosting, XGBoost, or LightGBM for improved performance.

Incorporate weather, traffic, and surge pricing features.

Deploy model via an API for real-time fare prediction.

Author

Harshit Sharma – Data Science / Machine Learning Developer
