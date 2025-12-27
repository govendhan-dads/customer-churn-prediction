# Customer Churn Prediction

## 📌 Project Overview
Customer churn is a critical challenge for subscription-based businesses.
This end-to-end data science project focuses on predicting customer churn
and translating technical insights into actionable business strategies.

---

## 📊 Dataset
- Telco Customer Churn Dataset (Kaggle)
- Contains customer demographics, services, billing details, and churn status
- Target variable: `Churn` (Yes / No)

---

## 🛠 Tools & Technologies
- Python 3.10
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🔍 Exploratory Data Analysis (EDA)
Key insights from data exploration:
- Customers on month-to-month contracts show higher churn
- Higher monthly charges are associated with increased churn
- Customers with shorter tenure are more likely to churn

![Churn by Contract](images/churn_by_contract.png)

---

## 🧹 Data Preprocessing
- Converted `TotalCharges` to numeric format
- Handled missing values
- Dropped non-informative identifier column (`customerID`)
- One-hot encoded categorical features
- Applied feature scaling for Logistic Regression
- Performed stratified train-test split

---

## 🤖 Model Training
Two machine learning models were trained and compared:

### Logistic Regression
- Used as a baseline model
- Feature scaling applied to ensure proper convergence

### Random Forest Classifier
- Used as the primary model
- Captures non-linear relationships effectively

---

## 📈 Model Performance
Random Forest outperformed Logistic Regression with better recall
and F1-score, making it more effective at identifying churn-prone customers.

![Confusion Matrix](images/confusion_matrix_rf.png)

---

## 🧠 Feature Importance
Key factors influencing churn:
- Contract type
- Customer tenure
- Monthly charges

---

## 💡 Business Recommendations
- Encourage customers to opt for long-term contracts
- Provide targeted retention offers to high-risk customers
- Focus retention strategies on newly onboarded customers

---

## 📁 Project Structure
~~~customer-churn-prediction/
~~~data/~~~
~~~notebooks/~~~
~~~images/~~~
~~~models/~~~
~~~README.md~~~
~~~requirements.txt

---

## ✅ Conclusion
This project demonstrates a complete data science workflow,
from data exploration and preprocessing to model building and
business insight generation.
