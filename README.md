# Car Price Prediction

This project explores various machine learning models to predict car prices based on a dataset containing car features and specifications.

## Project Goal

The primary goal of this project was to build a model that can accurately predict car prices. We explored several regression models and techniques to achieve the best possible performance.

## Dataset

The dataset used in this project is the "Car Price Prediction" dataset from Kaggle. It contains information about various cars, including their features and corresponding prices.

## Methodology

The project followed these general steps:

1.  **Data Loading and initial exploration:** Loaded the dataset and performed initial checks on its structure, data types, and basic statistics.
2.  **Feature Engineering:** Created new features from existing ones to potentially improve model performance. For example, extracting the car brand from the `CarName` column.
3.  **Data Cleaning and Preprocessing:** Handled categorical variables through one-hot encoding and prepared the data for model training.
4.  **Model Selection and Training:** Trained several regression models, including:
    *   Linear Regression
    *   Ridge Regression
    *   Lasso Regression
    *   Random Forest Regressor
    *   Neural Network
    *   Gradient Boosting
5.  **Model Evaluation:** Evaluated the performance of each model using metrics like Root Mean Squared Error (RMSE) and R-squared (R²).
6.  **Hyperparameter Tuning:** Attempted hyperparameter tuning for the Neural Network to optimize its performance.

## Key Observations on Accuracy

Achieving a very high R² (like 99%) on this dataset proved to be quite challenging. While techniques like feature engineering and hyperparameter tuning were applied, reaching near-perfect accuracy seems difficult with this data.

Interestingly, a relatively simple approach involving basic data cleaning and using a **Random Forest Regressor** yielded a good R² score (around 95%) which is competitive with many submissions on Kaggle. Pushing the accuracy beyond 95-96% appears to be tricky on this specific dataset, as also observed in the top Kaggle kernels.

It's important to note that while a high R² indicates the model explains a large portion of the variance in the target variable, it doesn't always guarantee the best prediction of the exact price values, especially with real-world data that might have inherent noise or uncaptured factors.

## Code

The code for this project is available in the Jupyter notebook in this repository. It includes the steps for data loading, preprocessing, model training, and evaluation.

## Leaderboard (if anyone wants to)

 Currently, the best R² achieved on this dataset in this repo is around 95% using a Random Forest Regressor, with up to 96% using a combination of several features. If you’d like, feel free to try improving the R².

| Rank | Contributor | R² Score | Model Used |
|------|------------|----------|------------|
| 1    | Unknown  | 0.95     | Random Forest Regressor |

- *Contributors: If you achieve a higher R², please submit your results via an Issue, Discussion, or Pull Request. The leaderboard will be updated accordingly.*
- *Note: R² indicates how well the model explains variance in prices, but does not guarantee exact price predictions.*

## Dataset / Related Work

- [Car Price Prediction dataset](https://www.kaggle.com/datasets/hellbuoy/car-price-prediction/data)
- [Top Kaggle Score 97% R²](https://www.kaggle.com/code/arjundoshi221/car-price-prediction-97)

