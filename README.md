# 💳 Credit Card Fraud Detection (Python | 2025)

📌 **Project Overview**
This end-to-end project tackles the critical challenge of detecting fraudulent credit card transactions using anonymized real-world data. It showcases a complete machine learning workflow — from data cleaning and exploratory analysis to class balancing (SMOTE), model evaluation, threshold tuning, and model serialization. This project simulates how a Data Analyst or Data Scientist would approach fraud risk in a real financial environment.

---

## 🔍 Business Questions

* 🛕️ Can we accurately identify fraudulent transactions from historical patterns?
* ⚖️ How do we handle highly imbalanced classes (only 0.17% are frauds)?
* 🤖 Which models perform best for this task (Logistic Regression, Random Forest)?
* 🌟 How can we maximize fraud detection without overwhelming false positives?
* 📈 What threshold provides the best balance between Precision and Recall?

---

## 🛠️ Tools & Libraries

| Tool/Library        | Purpose                            |
| ------------------- | ---------------------------------- |
| Python              | Core programming and analysis      |
| Pandas, NumPy       | Data wrangling and statistics      |
| Scikit-learn        | Modeling, metrics, preprocessing   |
| Imbalanced-learn    | SMOTE for oversampling fraud cases |
| Matplotlib, Seaborn | Data visualization                 |
| Joblib              | Saving trained models              |
| Git & GitHub        | Version control + portfolio        |

---

## 📊 Project Workflow

### 1. **Data Collection**

* 📂 Source: [Kaggle - Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
* 📈 284,807 total transactions
* ⚠️ Only 492 are fraudulent (\~0.17%) — extreme class imbalance

### 2. **Exploratory Data Analysis (EDA)**

* ✅ Checked for nulls, datatypes, duplicates — all clean
* 🔍 Transaction `Amount` is right-skewed with most under €100
* 🕒 `Time` feature shows cyclical patterns — fraud occurs uniformly
* 📊 Visualized class imbalance using count plots and log scales

### 3. **Data Preparation**

* 📏 Scaled `Amount` feature using `StandardScaler`
* 🧲 Train-test split using `stratify=y` to preserve class distribution
* 🥮 Applied **SMOTE** to oversample minority (fraud) class in training data

### 4. **Modeling & Evaluation**

#### 🔹 Logistic Regression (Baseline)

* 🚫 Detected very few fraud cases (recall \~60%)
* ✅ High precision but poor recall due to imbalance

#### 🔹 Logistic Regression + SMOTE

* ✅ Significantly improved recall (88%)
* ⚠️ Precision dropped — many false positives

#### 🔹 Random Forest Classifier + SMOTE

* 🌟 **Precision:** 78%
* 🌟 **Recall:** 89%
* 🌟 **F1 Score:** 83%
* 🌟 **ROC AUC:** 0.89
* ✅ Best model chosen for deployment

### 5. **Threshold Tuning**

* 📉 Evaluated performance at multiple decision thresholds
* 📈 Chose threshold that optimized F1 score
* 🧠 Final model caught 116 out of 148 frauds with 89% precision

### 6. **Model Export**

* 📂 Saved model using `joblib.dump()` for deployment:

```python
joblib.dump(rf_model, 'random_forest_fraud_model.pkl')
```

---

## 📈 Final Results

| Metric       | Score           |
| ------------ | --------------- |
| Precision    | 0.89            |
| Recall       | 0.78            |
| F1 Score     | 0.83            |
| ROC AUC      | 0.96            |
| Fraud Caught | 116 / 148 (78%) |

---

## ✅ Business Recommendations

* 🌟 Deploy model in real-time fraud monitoring systems
* ↺ Re-tune threshold periodically to adjust to fraud trends
* 🧪 Retrain monthly using new transactions for freshness
* 📊 Visualize fraud trends in Power BI or Tableau dashboards

---

## 📂 Folder Structure

```
credit-card-fraud-detection/
├── data/
│   └── creditcard.csv
├── notebooks/
│   └── credit_card_fraud_detection.ipynb
├── models/
│   └── random_forest_fraud_model.pkl
├── visuals/
│   ├── roc_auc.png
│   └── precision_recall_curve.png
└── README.md
```

---

## 📬 Let’s Connect

Hi! I'm **Olanrewaju Oyenekan**, actively seeking **Data Analyst / Junior Data Scientist roles (UK or Remote)**.

🔗 Explore more: [github.com/Larry0615](https://github.com/Larry0615)

---
