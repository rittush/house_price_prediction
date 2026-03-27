# House Price Prediction — Model Evaluation Report

## 📌 Project Overview
This project builds a Machine Learning model using **scikit-learn** to predict house prices based on property features.  
The pipeline includes data preprocessing, train-test splitting, model training, evaluation, and visualization.

---

## Model & Tools Used

| Component | Details |
|---|---|
| Language | Python |
| Libraries | pandas, numpy, scikit-learn, matplotlib, seaborn |
| Model | Linear Regression |
| Train-Test Split | 80% Training, 20% Testing |

---

## Data Preprocessing

- Missing numerical values filled using median
- Categorical values encoded using Label Encoding
- Features and target variable separated
- Target column: `price`

---

## Train-Test Strategy

The dataset was split using:

train_test_split(test_size=0.2, random_state=42)
Evaluation Setup
Dataset split: 80% Training / 20% Testing
Target variable: price
Evaluation performed on test set only to measure generalization

Metrics Used
Mean Absolute Error (MAE)

Average absolute difference between actual and predicted prices.

MAE = mean(|y_true - y_pred|)

Interpretation: On average, predictions differ from actual prices by MAE units.

Mean Squared Error (MSE)

Average squared difference between actual and predicted prices.

MSE = mean((y_true - y_pred)^2)

Interpretation: Penalizes larger errors more than MAE.

Root Mean Squared Error (RMSE)

Square root of MSE.

RMSE = sqrt(MSE)

Interpretation: Error in the same units as house price.

R² Score (Coefficient of Determination)

Measures how well the model explains the variance in house prices.

R2 = 1 - (SS_res / SS_tot)
