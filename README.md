# 📞 telecom-customer-churn-prediction

A machine learning project to identify customers likely to churn, generate churn risk scores, and provide actionable business insights for proactive retention strategies.

---

## 🎯 Project Objectives

* Identify customers at risk of churn
* Generate churn probability scores
* Segment customers into risk groups
* Understand key drivers of churn
* Provide business recommendations for retention

---

## 📊 Dataset

The dataset is loaded from a telecom SQL database and contains customer usage patterns, plan details, service interactions, and churn labels.

**Key Features**

* Call minutes & charges (Day, Evening, Night, International)
* Customer service calls
* Voicemail & international plans
* Account length & usage behavior
* Target variable: **CHURN_FLAG**

---

## ⚙️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Seaborn, Matplotlib
* PyMySQL
* Jupyter Notebook

---

## 🔎 Project Workflow

### ✅ Data Collection

* Loaded telecom customer data from SQL database

### ✅ Data Cleaning

* Standardized churn labels
* Converted object columns to numeric
* Handled missing values with median imputation

### ✅ Feature Engineering

* Created binary churn flag
* One-hot encoded categorical variables
* Scaled numerical features

### ✅ Modeling

Two models were trained:

* Logistic Regression (baseline)
* Random Forest (final model)

### ✅ Evaluation

Metrics used:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC

---

## ⭐ Model Results

### Logistic Regression

* Accuracy: **86%**
* Recall (churn): **23%**
* ROC-AUC: **0.79**

### Random Forest (Final Model)

* Accuracy: **94%**
* Recall (churn): **60%**
* ROC-AUC: **0.89**

👉 Random Forest selected as best model.

---

## 🔥 Key Churn Drivers

Top predictors identified:

1. Customer Service Calls
2. Day Minutes & Charges
3. International Plan
4. Evening Minutes & Charges
5. International Usage

---

## 🎯 Customer Risk Segmentation

Customers classified into:

* **High Risk** → churn score ≥ 0.70
* **Medium Risk** → churn score 0.40–0.69
* **Low Risk** → churn score < 0.40

---

## 💼 Business Recommendations

* Improve customer support for high call-frequency customers
* Optimize pricing for heavy usage customers
* Reevaluate international plan offerings
* Implement proactive retention campaigns using churn scores
* Use segmentation for targeted marketing

---

## 🚀 How to Run

```bash
# Clone repository
git clone https://github.com/SyedHussain23/telecom-customer-churn-prediction.git

# Navigate to project folder
cd telecom-customer-churn-prediction

# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook telecom-customer-churn-prediction.ipynb
```

---

## ⚠️ Database Setup

Update SQL credentials before running:

```python
HOST = "your_host"
USER = "your_user"
PASSWORD = "your_password"
DB_NAME = "your_database"
```

👉 For security, store credentials using `.env` file.

---

## 📂 Project Output

The project generates:

* Churn predictions
* Churn probability scores
* Risk segmentation
* Business-ready dataset

```
telecom_churn_predictions.csv
```

---

## 🔮 Future Improvements

* Hyperparameter tuning
* Advanced ensemble models (XGBoost, LightGBM)
* Deep learning churn modeling
* Real-time churn prediction pipeline
* Deployment via API or dashboard

---

## 👨‍💻 Author

**Syed Hussain Abdul Hakeem**

🔗 GitHub: [https://github.com/SyedHussain23](https://github.com/SyedHussain23)
🔗 LinkedIn: [[https://www.linkedin.com/in/syedhussain23](https://www.linkedin.com/in/syedhussain23)](https://www.linkedin.com/in/syed-hussain-abdul-hakeem)

---

## ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.
