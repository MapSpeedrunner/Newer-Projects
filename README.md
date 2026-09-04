# House Price Prediction using Orange Data Mining

## Overview

This project uses **Orange Data Mining** to build and evaluate machine learning models for predicting house prices.

The workflow demonstrates a complete regression pipeline, starting with data preparation and feature selection, followed by exploratory analysis, train/test splitting, model training, evaluation, and prediction.

## Dataset

The project uses the **USA Housing** dataset containing information about houses and their corresponding prices.

The selected features include:

- Income
- House Age
- Number of Rooms
- Number of Bedrooms
- Area Population

The target variable is:

- Price

## Machine Learning Workflow

The Orange workflow consists of:

1. **Data Loading** – Importing the USA Housing dataset.
2. **Feature Selection** – Selecting relevant variables for prediction.
3. **Exploratory Data Analysis** – Using Data Table, Rank, Box Plot, and Distributions.
4. **Train/Test Split** – Using Data Sampler to create a 4,000-row training set and a 1,000-row test set.
5. **Model Training** – Comparing three regression algorithms:
   - Linear Regression
   - Random Forest
   - k-Nearest Neighbors (kNN)
6. **Model Evaluation** – Comparing the models using Test & Score.
7. **Prediction** – Generating predictions for the held-out test data.
8. **Visualization** – Comparing actual house prices with Linear Regression predictions using a scatter plot.

## Results

The models were evaluated on the 1,000-row test set.

| Model | RMSE | MAE | MAPE | R² |
|---|---:|---:|---:|---:|
| **Linear Regression** | **100,059.727** | **80,269.567** | **7.640** | **0.924** |
| Random Forest | 123,433.206 | 97,192.905 | 12.014 | 0.885 |
| kNN | 249,558.393 | 201,435.983 | 22.678 | 0.530 |

### Best Model

**Linear Regression** performed best on the held-out test set, achieving:

- **RMSE:** 100,059.727
- **MAE:** 80,269.567
- **R²:** 0.924

The results indicate that Linear Regression provided the strongest predictive performance among the three tested models for this dataset.

## Project Files

- `USA_Housing.csv` — Dataset used by the workflow.
- `house_price_prediction.ows` — Complete Orange Data Mining workflow.
- Screenshots — Visual documentation of the workflow, model comparison, and predictions.

## Tools Used

- Orange Data Mining
- Linear Regression
- Random Forest
- k-Nearest Neighbors (kNN)
- Regression evaluation metrics
