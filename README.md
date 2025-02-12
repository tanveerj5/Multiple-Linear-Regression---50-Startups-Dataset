# Multiple Linear Regression - 50 Startups Dataset

This project applies **Multiple Linear Regression** to predict the **Profit** of a startup based on various factors such as **R&D Spend, Administration, Marketing Spend, and State**, using the **50 Startups dataset**.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Libraries Required](#libraries-required)
3. [Dataset](#dataset)
4. [Steps for Training the Model](#steps-for-training-the-model)
    - [Step 1: Importing Libraries](#step-1-importing-libraries)
    - [Step 2: Loading the Dataset](#step-2-loading-the-dataset)
    - [Step 3: Encoding Categorical Data](#step-3-encoding-categorical-data)
    - [Step 4: Avoiding the Dummy Variable Trap](#step-4-avoiding-the-dummy-variable-trap)
    - [Step 5: Splitting the Dataset into Training and Test Sets](#step-5-splitting-the-dataset-into-training-and-test-sets)
    - [Step 6: Feature Scaling](#step-6-feature-scaling)
    - [Step 7: Training the Model](#step-7-training-the-model)
    - [Step 8: Making Predictions](#step-8-making-predictions)
    - [Step 9: Evaluating Model Performance](#step-9-evaluating-model-performance)
5. [Conclusion](#conclusion)

---

## Project Overview
The goal of this project is to predict the **Profit** of a startup using **Multiple Linear Regression**. The dataset contains **50 startups** and includes **features** such as:
- **R&D Spend**
- **Administration**
- **Marketing Spend**
- **State** (Categorical variable)

We train a **Multiple Linear Regression model** and evaluate its performance using various metrics such as **Mean Squared Error (MSE), Mean Absolute Error (MAE), and R-squared (R²)**.

---

## Metric Score
![alt text](https://github.com/tanveerj5/Multiple-Linear-Regression---50-Startups-Dataset/blob/main/score.png)

## Assumptions of Linear Regression
![alt text](https://github.com/tanveerj5/Multiple-Linear-Regression---50-Startups-Dataset/blob/main/Assumptions%20of%20Linear%20Regression.png)

## Libraries Required
To run this project, the following libraries are required:

```python
import pandas as pd      # For data manipulation
import numpy as np       # For numerical operations
from sklearn.compose import ColumnTransformer
from sklearn.preprocessing import OneHotEncoder, StandardScaler
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error, mean_absolute_error, r2_score
