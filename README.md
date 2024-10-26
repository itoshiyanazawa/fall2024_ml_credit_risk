# Credit Risk Modeling Project

## Overview

This project focuses on building a credit risk model and designing a strategy to assign credit. We use machine learning techniques to predict the probability of default for credit card applicants and develop strategies for credit approval.

## Data

The project uses data from the [American Express - Default Prediction](https://www.kaggle.com/competitions/amex-default-prediction/data) Kaggle competition. We work with two main files:

- `train_data.csv`: Contains customer activity data for the 13 months leading up to April 2018.
- `train_labels.csv`: Shows the default status of customers as of April 2018 (target variable).

Due to the large size of the dataset, we use a 20% random sample for development.

## Project Structure

1. Data Preparation
   - Random sampling of 20% observations
   - Merging sampled data with customer activity data
   - One-hot encoding of categorical variables

2. Feature Engineering
   - Aggregation of numerical features (e.g., average, sum, min, max)
   - Aggregation of categorical features (e.g., response rates)

3. Model Development
   - XGBoost model
     - Feature importance analysis
     - Grid search for hyperparameter tuning
   - Neural Network model
     - Data preprocessing (missing value imputation, outlier treatment, normalization)
     - Grid search for architecture and hyperparameters

4. Model Evaluation
   - Performance comparison between XGBoost and Neural Network models
   - Analysis using SHAP values for XGBoost model

5. Strategy Development
   - Conservative and aggressive approval strategies
   - Portfolio default rate and revenue estimation

## Key Components

- Feature selection based on importance
- Hyperparameter tuning for both XGBoost and Neural Network models
- SHAP analysis for model interpretability
- Custom function for strategy evaluation

## Results

The project delivers:
- An optimized credit risk model (either XGBoost or Neural Network)
- Two credit approval strategies (conservative and aggressive)
- Estimated portfolio default rates and revenues for each strategy

## Presentation

The results are summarized in a comprehensive presentation, including:
- Executive summary
- Data overview and feature engineering process
- Model development and evaluation details
- Strategy recommendations with supporting analysis

## Requirements

- Python 3.x
- Libraries: pandas, numpy, scikit-learn, xgboost, tensorflow, shap
- Jupyter Notebook (for development and analysis)

## Usage

1. Clone the repository
2. Download the data from the Kaggle competition link provided above
3. Run the Jupyter notebooks in sequence to reproduce the analysis

## Note

This project is designed for educational purposes and may require adjustments for production use.
