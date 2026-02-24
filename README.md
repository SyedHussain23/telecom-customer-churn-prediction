# 📞 telecom-customer-churn-prediction

## 📌 Project Overview

Customer churn is a major challenge in the telecom industry due to intense competition and customer switching behavior.
This project builds a **machine learning solution** to predict churn risk and provide actionable insights for retention strategies.

The business objective is to:

✅ Identify customers likely to churn
✅ Generate churn probability scores
✅ Segment customers into risk groups
✅ Discover key churn drivers for business action

This aligns with the No-Churn Telecom business case where ML is used to understand churn variables and create predictive churn flags for retention campaigns. 

---

## 🎯 Business Goals

* Understand variables influencing customer migration
* Create **CHURN_FLAG (0/1)** prediction
* Provide churn risk scores for targeted campaigns
* Support proactive customer retention

---

## 📊 Dataset

The dataset was loaded directly from a **SQL database** containing telecom customer usage and service information including:

* Customer demographics
* Plan subscriptions
* Usage metrics (minutes, calls, charges)
* Customer service interactions
* Churn label

---

## ⚙️ Project Workflow

### 1️⃣ Data Loading

* Connected to SQL database using PyMySQL
* Extracted telecom churn dataset

### 2️⃣ Data Cleaning

* Standardized churn column formats
* Created **CHURN_FLAG**
* Converted numeric columns
* Median imputation for missing values

### 3️⃣ Feature Engineering

* Numeric vs categorical separation
* One-hot encoding
* Standard scaling

### 4️⃣ Model Building

Two models were trained:

✅ Logistic Regression (baseline)
✅ Random Forest (final model)

### 5️⃣ Model Evaluation

Metrics used:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC
* Confusion Matrix

---

## 🏆 Model Performance

### 🔹 Logistic Regression

* Accuracy: **86%**
* Recall (churn): **23%**
* ROC-AUC: **0.79**

👉 Missed many churners

---

### 🔹 Random Forest (Final Model)

* Accuracy: **94%**
* Recall (churn): **60%**
* F1-score: **73%**
* ROC-AUC: **0.89**

👉 Strong churn detection and overall performance

---

## ⭐ Key Churn Drivers

Random Forest feature importance revealed:

1️⃣ Customer Service Calls
2️⃣ Day Minutes & Charges
3️⃣ International Plan
4️⃣ Evening Usage
5️⃣ International Charges

👉 Service issues and usage cost are primary churn factors

---

## 📊 Churn Risk Segmentation

Customers were segmented using predicted probabilities:

* 🔴 High Risk (≥ 0.7)
* 🟡 Medium Risk (0.4–0.7)
* 🟢 Low Risk (< 0.4)

This enables targeted retention strategies.

---

## 💼 Business Recommendations

* Improve support for customers with frequent service calls
* Optimize pricing for high usage customers
* Re-evaluate international plan value
* Use churn scores for proactive retention campaigns

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* PyMySQL
* Matplotlib, Seaborn
* SQL Database

---

## 🚀 Future Improvements

* Hyperparameter tuning
* Gradient boosting / XGBoost
* Deep learning churn modeling
* Real-time churn prediction pipeline
* Customer lifetime value integration

---

## 👨‍💻 Author

**Syed Hussain Abdul Hakeem**

🔗 GitHub: [https://github.com/SyedHussain23](https://github.com/SyedHussain23)
🔗 LinkedIn: [https://linkedin.com/in/syed-hussain-abdul-hakeem](https://linkedin.com/in/syed-hussain-abdul-hakeem)

---

⭐ If you found this project useful, please consider giving it a **star** on GitHub!
