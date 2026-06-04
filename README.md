# Fraud-Detection-Assignment-
Fraud Detection Assignment submission including data analysis, preprocessing, modeling, and evaluation 

| Model | AUC-ROC | F1 | Fraud Recall |
|---|---|---|---|
| Logistic Regression | 0.9917 | 0.71 | 59% |
| Random Forest | 0.9461 | 0.72 | 65% |
| XGBoost | 0.9732 | 0.71 | 62% |
| XGBoost + SMOTE | 0.9921 | 0.69 | 76% |
| **XGBoost + SMOTE + Tuning** ✅ | **0.9922** | **0.69** | **76%** |

## Pipeline

1. Data Preprocessing — stripped quotes, handled unknowns, dropped zero-variance & ID columns
2. Feature Engineering — `time_of_day` from step, OHE encoding, StandardScaler on amount
3. EDA — fraud patterns by category, amount, gender, age, hour
4. Model Training — Logistic Regression, Random Forest, XGBoost
5. Model Interpretation — feature importance
6. SMOTE — synthetic oversampling on training data only 
7. Hyperparameter Tuning — RandomizedSearchCV, 20 iterations, 3-fold CV


Place `fraud.csv` in the same folder and run all cells top to bottom.
