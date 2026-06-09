# synent-task8-mlmodel-yourname

## Problem Statement

Predicting house prices is a common real-world problem where many factors like size, location, and quality all play a role. The goal was to build a machine learning model that can predict the sale price of a house given its features.

## Dataset Details

- Dataset: House Price Dataset
- Source: Kaggle
- Contains around 80 features describing residential homes including lot area, overall quality, year built, basement area, living area, number of bathrooms, garage capacity, and the sale price as the target.
- Format: CSV

## Approach

I started by handling missing values and encoding categorical columns. A correlation heatmap helped me pick the top features most related to sale price. I selected around 15 features for the final model. The data was split 80/20 into training and test sets. I trained three models: Linear Regression as a baseline, a Decision Tree, and a Random Forest. Each model was evaluated using RMSE and R squared score on the test set.

## Results

| Model | RMSE | R2 Score |
|---|---|---|
| Linear Regression | ~35000 | 0.78 |
| Decision Tree | ~28000 | 0.83 |
| Random Forest | ~21000 | 0.91 |

- Random Forest performed best with the lowest error
- Overall quality, ground floor living area, and garage capacity were the most important features
