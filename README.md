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

```python
train_test_split(test_size=0.2, random_state=42)
