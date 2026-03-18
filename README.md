# Rainfall Prediction App Using Machine Learning in Python

This project predicts whether rainfall will occur using machine learning classification models based on historical weather data.

📌 Project Overview

The dataset contains daily weather parameters such as pressure, temperature, humidity, cloud cover, sunshine, wind direction, and wind speed.
The goal is to predict rainfall occurrence ("yes" or "no") using supervised machine learning.

📂 Dataset Information

- Total records: 366
- Total features: 12
- Target variable: "rainfall"

⚙️ Data Preprocessing

- Removed extra spaces from column names
- Handled missing values using mean imputation
- Converted rainfall labels:
  - yes → 1
  - no → 0
- Removed highly correlated features:
  - maxtemp
  - mintemp
- Applied feature scaling using StandardScaler
- Balanced dataset using RandomOverSampler

🤖 Machine Learning Models Used

- Logistic Regression
- XGBoost Classifier
- Support Vector Machine (SVC)

📊 Model Performance (ROC-AUC Validation Score)

- Logistic Regression: 0.8967
- XGBoost Classifier: 0.8392
- SVC: 0.8858

✅ Best Performing Model

Logistic Regression gave the highest validation score.

📈 Evaluation Methods

- ROC-AUC Score
- Confusion Matrix
- Classification Report

🛠 Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Imbalanced-learn

📁 Files Included

- rainfall_prediction.ipynb
- Rainfall.csv

🎯 Objective

To build a machine learning model that predicts rainfall using weather conditions.

🚀 Future Improvement

- Deploy as web app using Streamlit
- Test on larger datasets
- Improve model generalization
