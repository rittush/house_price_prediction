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
Metrics used:
Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R² Score
Evaluation Metrics
1️ Mean Absolute Error (MAE)

Definition:
Average absolute difference between actual and predicted prices.


Interpretation:
On average, predictions are off by MAE price units.

2️ Mean Squared Error (MSE)

Definition:
Average squared difference between actual and predicted prices.

Interpretation:
Penalizes large errors more heavily than MAE.

3️ Root Mean Squared Error (RMSE)

Definition:
Square root of MSE.

𝑅
𝑀
𝑆
𝐸
=
𝑀
𝑆
𝐸
RMSE=
MSE
	​


Interpretation:
Represents prediction error in the same units as price, making it easier to understand.

4️ R² Score (Coefficient of Determination)

Definition:
Measures how well the model explains the variance in house prices.

