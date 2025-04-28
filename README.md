# Housing Price Prediction using Linear Regression

## Overview
This project implements simple and multiple linear regression models to predict housing prices based on various features. The task was completed as part of an AI & ML internship program to demonstrate understanding of linear regression concepts, evaluation metrics, and model interpretation.

## Dataset
The project uses the [Housing Price Prediction dataset](https://www.kaggle.com/datasets/harishkumardatalab/housing-price-prediction) from Kaggle, which contains:
- 545 observations
- 12 features (both numerical and categorical)
- Target variable: House price

Key features include:
- `area`: Total area in square feet
- `bedrooms`, `bathrooms`: Number of each
- `stories`: Number of floors
- Various amenities (air conditioning, basement, etc.)
- `furnishingstatus`: Quality of furnishings

## Implementation Steps

1. **Data Preprocessing**:
   - Encoded categorical variables (yes/no → 1/0)
   - Label encoded furnishing status
   - Handled missing values (none found in this dataset)

2. **Simple Linear Regression**:
   - Used only `area` to predict price
   - Achieved R² score of 0.28

3. **Multiple Linear Regression**:
   - Used all relevant features
   - Achieved R² score of 0.65
   - Identified most important features

4. **Evaluation**:
   - Calculated MAE, MSE, and R² scores
   - Analyzed residuals
   - Visualized actual vs predicted values

## Results

### Simple Regression (Area vs Price)
| Metric | Value |
|--------|-------|
| MAE    | 1,153,000 |
| MSE    | 2.12e+12 |
| R²     | 0.28 |

![Simple Regression Plot](images/simple_regression.png)

### Multiple Regression
| Metric | Value |
|--------|-------|
| MAE    | 738,000 |
| MSE    | 1.03e+12 |
| R²     | 0.65 |

Top 3 Most Important Features:
1. Area (coefficient: +366.85)
2. Bathrooms (coefficient: +825,000)
3. Air Conditioning (coefficient: +623,000)

![Multiple Regression Plot](images/multiple_regression.png)
