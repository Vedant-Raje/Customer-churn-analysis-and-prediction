# 📊 Customer Churn Analysis & Prediction Using Machine Learning

## 🔎 Overview

Customer churn is a critical business challenge for subscription-based companies, as losing customers directly impacts revenue and growth.

This project analyzes customer behavior and builds machine learning models to predict churn, enabling businesses to proactively identify and retain at-risk customers.

The project covers:

- Data cleaning and preprocessing  
- Exploratory Data Analysis (EDA)  
- Feature engineering  
- Classification modeling  
- Model evaluation  
- Business insights and recommendations  

---

## 🎯 Objective

The objective of this project is to:

- Identify patterns influencing customer churn  
- Develop predictive models to classify customers as churned or retained  
- Provide actionable recommendations to improve customer retention  

---

## 📁 Dataset

- **Dataset:** Telco Customer Churn Dataset  
- **Source:** Kaggle  
- **Size:** ~7,000 customer records  
- **Target Variable:** `Churn` (Yes / No)

### Features include:

- Customer demographics  
- Service subscriptions  
- Contract type  
- Billing information  
- Tenure  
- Payment method  

---

## 🛠 Project Workflow

### 1️⃣ Data Cleaning

- Converted `TotalCharges` to numeric format  
- Handled missing values using median imputation  
- Removed irrelevant identifier (`customerID`)  
- Encoded categorical variables using one-hot encoding  

---

### 2️⃣ Exploratory Data Analysis (EDA)

Key analyses performed:

- Overall churn distribution  
- Churn vs contract type  
- Churn vs tenure  
- Churn vs monthly charges  
- Correlation analysis  

#### Key Observations:

- Customers with month-to-month contracts have significantly higher churn rates  
- Customers with shorter tenure are more likely to churn  
- Higher monthly charges show positive correlation with churn  

---

### 3️⃣ Feature Engineering

- Encoded categorical features  
- Split dataset into training and testing sets (80/20 split)  
- Addressed class imbalance using class weighting / SMOTE (if applied)  

---

### 4️⃣ Model Building

Implemented and compared:

- Logistic Regression  
- Random Forest Classifier  

---

### 5️⃣ Model Evaluation

Evaluation metrics used:

- Confusion Matrix  
- Precision  
- Recall  
- F1-Score  
- ROC-AUC Score  

Special focus was placed on **Recall**, as failing to identify churners can lead to revenue loss.

---

## 📈 Model Performance

| Model | Accuracy | Recall (Churn) | ROC-AUC |
|--------|----------|----------------|--------|
| Logistic Regression | 82% | 60% | 0.862 |
| Random Forest (Balanced) | 77% | 83% | 0.866 |

---

## 🔍 Feature Importance

The most influential features for churn prediction include:

- Tenure  
- Total Charges  
- Contract type  
- Monthly charges  

These variables significantly influence customer retention behavior.

---

## 💡 Business Insights & Recommendations

### Key Findings:

- Month-to-month contract customers are at highest risk of churn  
- Short-tenure customers churn more frequently  
- Customers with higher monthly charges show increased churn probability  

### Business Recommendations:

- Offer incentives for long-term contracts  
- Improve onboarding experience for new customers  
- Identify high-risk customers for targeted retention campaigns  
- Implement loyalty benefits for long-term customers  

---

## ▶ How to Run the Project

1. Clone the repository:

```bash
git clone https://github.com/yourusername/customer-churn-analysis.git
```
2. Install Dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook:

   ```bash
   jupyter notebook
   ```


