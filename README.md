# Customer_Churn_Prediction
Developed the models for Customer Churn Prediction as an Internship work at Codec Technologies 

# Customer Churn Prediction

## Project Overview
Customer churn prediction is a crucial task for businesses, particularly in the telecom industry, to identify customers who are likely to stop using their services. This project uses machine learning models to predict customer churn based on the Telco Customer Churn dataset. The main goal is to enable proactive retention strategies to reduce churn and increase customer lifetime value.

---

## Dataset
- **Dataset Name:** Telco Customer Churn  
- **Source:** Kaggle  
- **File:** `Telco_customer_churn.xlsx`  
- **Description:** Contains customer demographics, account information, services subscribed, and churn information.  
- **Rows:** 7043  
- **Columns:** 33  

---

## Features
Some important features used in the dataset include:  

- **Demographics:** Gender, Senior Citizen, Partner, Dependents  
- **Account Info:** Tenure Months, Monthly Charges, Total Charges, CLTV  
- **Services:** Phone Service, Multiple Lines, Internet Service, Online Security, Tech Support, Streaming Services  
- **Payment & Contract:** Contract Type, Payment Method, Paperless Billing  

---

## Preprocessing Steps
1. Handle missing values in numerical and categorical columns.  
2. Convert categorical columns to numerical using one-hot encoding and label mapping.  
3. Scale numerical features using `StandardScaler`.  
4. Split dataset into training and testing sets (70:30 ratio).  

---

## Machine Learning Models Used
- **Logistic Regression**  
- **Random Forest Classifier**  
- **XGBoost Classifier**  

**Model Evaluation Metrics:**  
- Accuracy  
- Recall  
- Precision  
- F1-score  
- ROC-AUC  

---

## Results
| Model                | Accuracy | Recall | ROC-AUC |
|----------------------|----------|--------|---------|
| Logistic Regression  | 0.909    | 0.911  | 0.974   |
| Random Forest        | 0.908    | 0.802  | 0.957   |
| XGBoost              | 0.921    | 0.865  | 0.981   |

**Insights:**  
- Customers with **month-to-month contracts** and **short tenure** are more likely to churn.  
- Higher **Monthly Charges** and lower **CLTV** increase churn probability.  
- XGBoost performed the best and is suitable for deployment.  

---

## Files in the Repository
- `Customer_churn_prediction.ipynb` → Jupyter Notebook containing code, EDA, preprocessing, modeling, and evaluation.  
- `Customer_churn_prediction_Report.pdf` → Project report with methodology, results, and discussions.  
- `Telco_customer_churn.xlsx` → Dataset used for modeling.  
- `logistic_churn_model.pkl` → Trained Logistic Regression model.  
- `xgboost_churn_model.pkl` → Trained XGBoost model.  
- `README.md` → This file.  

---

## How to Run
1. Clone the repository.  
2. Install required Python libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost joblib

---

## Author

Divesh Sonawane

Email: diveshsonawane66@gmail.com
