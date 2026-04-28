# food-delivery-time-prediction
Courier's food delivery time prediction project based on the Machine Learning Boosting Trees model (XGBoost library)

# Food Delivery Time Prediction
Predicting food delivery time using gradient boosted trees (XGBoost), 
built as part of a Kaggle mini-competition. Final private leaderboard 
MAPE: **0.1465**.

## Models Compared
| Model | Validation MAPE |
|---|---|
| Lasso Regression | 0.2148 |
| Random Forest | 0.1456 |
| XGBoost (final) | 0.1412 |

## Key Features Engineered
- **Haversine distance** from restaurant to delivery coordinates
- **Log-transform on target** to optimize for relative error (MAPE) 
  rather than absolute error
- Time-of-day flags: rush hour, lunch, dinner, late night
- Interaction features: effective distance (km × traffic intensity), 
  rider experience (rating × age), congestion batch impact
- Weather severity label encoding, missing value indicators

## Tech Stack
Python, XGBoost, scikit-learn, pandas, NumPy, Matplotlib
