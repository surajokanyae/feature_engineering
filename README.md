# NBA Player Longevity Prediction: Feature Engineering

## Project Overview
This project focuses on analyzing NBA player performance data to engineer features for a machine learning model aimed at predicting player longevity in the league. Using Python and the pandas library, we transform raw sports statistics into model-ready inputs, focusing on defining target variables, removing noise, analyzing correlations, creating composite metrics, and handling missing data.

## Dataset Source
The dataset used for this analysis is `nba-players.csv`. This file contains various statistics for NBA players.

## Prediction Goal
The primary objective of this project is to predict whether an NBA player will last more than 5 years in the league. This is captured by the `target_5yrs` column in the dataset, which serves as our dependent variable.

## Feature Engineering Workflow
The following steps have been undertaken to prepare the dataset for predictive modeling:

1.  **Dataset Loading and Target Definition**: The `nba-players.csv` dataset was loaded into a pandas DataFrame. The `target_5yrs` column was explicitly defined as the dependent variable for longevity prediction.

2.  **Removal of Non-Predictive Columns**: Irrelevant and potentially noise-introducing columns such as `'Unnamed: 0'` (an arbitrary index) and `'name'` (player names) were dropped from the dataset to prevent data leakage and improve model focus.

3.  **Correlation Analysis**: A comprehensive correlation analysis was performed. This involved examining the relationships between all features and the `target_5yrs` variable, as well as identifying highly correlated features among themselves to address potential multicollinearity.

4.  **Composite Feature Engineering**: A new meaningful composite feature, 'Points Per Minute' (`ppm`), was engineered. This metric calculates a player's average points scored per minute played, providing a normalized measure of offensive efficiency.

5.  **Handling Missing Values**: The dataset was inspected for null values. It was confirmed that there are no missing values in the performance columns, ensuring the dataset's integrity and readiness for machine learning algorithms.

This systematic approach to feature engineering aims to produce a clean, robust, and predictive dataset for forecasting NBA player. longevity.
```
