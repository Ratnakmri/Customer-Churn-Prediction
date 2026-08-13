# Customer Churn Prediction

## 📌 Project Overview

Customer churn prediction is the process of identifying customers who are likely to stop using a company's services.

This project uses machine learning techniques to predict customer churn using the Telco Customer Churn dataset. Exploratory Data Analysis (EDA) was performed to identify important churn patterns, followed by training and evaluation of three classification models.

## 🎯 Objectives

- Analyze customer churn patterns
- Perform data cleaning and preprocessing
- Explore factors associated with customer churn
- Build machine learning classification models
- Compare model performance using Accuracy, Recall, and ROC-AUC
- Identify important features influencing churn predictions

## 📂 Dataset

The project uses the Telco Customer Churn dataset containing customer demographic, service, contract, and billing information.

After cleaning:

- Records: 7,032
- Features: 19
- Target: Churn

### Target Distribution

- No Churn: 5,163
- Churn: 1,869
- Churn Rate: 26.6%

## 🔍 Exploratory Data Analysis

The analysis examined:

- Customer churn distribution
- Churn percentage
- Churn by contract type
- Customer tenure vs churn
- Monthly charges vs churn

### Key Findings

- Month-to-month customers show substantially higher churn than customers with one-year or two-year contracts.
- Customers with shorter tenure are more likely to churn.
- Churned customers tend to have higher monthly charges.
- Tenure, total charges, contract type, and monthly charges are among the most important features used by the Random Forest model.

## 🤖 Machine Learning Models

Three classification models were trained:

1. Logistic Regression
2. Random Forest
3. XGBoost

## 📊 Model Performance

| Model | Accuracy | Recall | ROC-AUC |
|---|---:|---:|---:|
| Logistic Regression | 80.38% | 57.22% | 83.59% |
| Random Forest | 77.26% | 63.64% | 82.53% |
| XGBoost | 78.89% | 52.94% | 83.26% |

## 🏆 Model Analysis

Logistic Regression achieved the highest overall Accuracy and ROC-AUC among the three models.

Random Forest achieved the highest Recall, making it useful when the objective is to identify a larger proportion of customers who are likely to churn.

The choice of model therefore depends on the business objective.

## 📈 Model Evaluation

The models were evaluated using:

- Accuracy
- Recall
- ROC-AUC
- Confusion Matrix
- ROC Curve
- Feature Importance

## 💡 Business Insights

Based on the analysis, businesses could:

- Focus retention campaigns on month-to-month customers.
- Provide additional support during the early stages of the customer lifecycle.
- Investigate pricing and service value for customers with higher monthly charges.
- Encourage customers to move toward longer-term contracts.
- Monitor customers with characteristics associated with higher churn risk.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook / Google Colab

## 📁 Project Structure

Customer-Churn-Prediction/

├── data/

│   └── Telco-Customer-Churn.csv

├── notebooks/

│   └── customer_churn_prediction.ipynb

├── images/

├── README.md

└── requirements.txt

## 🚀 How to Run

1. Clone the repository.
2. Install the required libraries:

```bash
pip install -r requirements.txt
