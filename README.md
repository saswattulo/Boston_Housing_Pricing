# Boston Housing Price Prediction

## Project Overview

This repository contains a Jupyter notebook for predicting housing prices in Boston using various machine learning models. The project involves data preprocessing, model training, hyperparameter tuning, and evaluation using metrics like Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² Score.

## Dataset

The dataset used in this project is the Boston Housing dataset, which contains information about housing prices and various features of homes in Boston. The features include:
- `crim`: Per capita crime rate by town
- `zn`: Proportion of residential land zoned for lots over 25,000 sq. ft.
- `indus`: Proportion of non-retail business acres per town
- `chas`: Charles River dummy variable (1 if tract bounds river; 0 otherwise)
- `nox`: Nitric oxides concentration (parts per 10 million)
- `rm`: Average number of rooms per dwelling
- `age`: Proportion of owner-occupied units built prior to 1940
- `dis`: Weighted distances to five Boston employment centers
- `rad`: Index of accessibility to radial highways
- `tax`: Full-value property tax rate per $10,000
- `ptratio`: Pupil-teacher ratio by town
- `b`: \(1000(Bk - 0.63)^2\) where Bk is the proportion of Black residents by town
- `lstat`: Percentage of lower status of the population
- `medv`: Median value of owner-occupied homes in $1000s (target variable)

## Methodology

1. **Data Preprocessing**:
   - Loaded and examined the dataset.
   - Split the data into training and testing sets.
   - Scaled the features using `StandardScaler`.

2. **Model Training**:
   - Trained various models including:
     - Linear Regression
     - RidgeCV
     - LassoCV
     - ElasticNet
     - Ridge
     - Lasso
     - Decision Tree
     - Random Forest
     - XGBoost
   - Evaluated models using Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² Score.

3. **Hyperparameter Tuning**:
   - Tuned the hyperparameters of the XGBoost model to improve performance.

## Results

- **XGBoost** achieved the best performance with the following metrics:
  - MAE: 1.964606
  - MSE: 7.124317
  - R²: 0.902851

## Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/boston-housing-price-prediction.git
