# 💳 Credit Card Fraud Detection (Python | 2025)

📌 **Project Overview**  
This end-to-end project focuses on detecting fraudulent credit card transactions using real-world data. It applies advanced feature engineering, data balancing techniques, and supervised machine learning models to classify rare fraud cases. The goal is to simulate how a Data Analyst or Data Scientist would approach fraud risk in a financial services context.

---

## 🔍 Business Questions

- 🕵️‍♂️ Can we accurately classify fraud using transaction patterns?
- ⚖️ How do we deal with extremely imbalanced classes?
- 🧠 Which machine learning models perform best for fraud detection?
- 📊 How can we visualize results to help stakeholders?

---

## 🛠️ Tools & Libraries

| Tool/Library     | Purpose                              |
|------------------|---------------------------------------|
| Python           | Core programming and analysis         |
| Pandas, NumPy    | Data wrangling                       |
| Scikit-learn     | Modeling, evaluation, preprocessing   |
| Imbalanced-learn | SMOTE, undersampling                 |
| Matplotlib, Seaborn | Visualizations                    |
| Streamlit (optional) | Interactive fraud prediction demo |
| Git & GitHub     | Version control and collaboration     |

---

## 📊 Project Workflow

1. **Data Collection**  
   - Source: [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
   - 284,807 transactions | 492 frauds (~0.17%)

2. **EDA**  
   - Distribution, correlations, and transaction behavior

3. **Data Prep & Feature Engineering**  
   - Feature scaling  
   - Handling imbalance with SMOTE/undersampling  
   - Train/test split (stratified)

4. **Modeling & Evaluation**  
   - Models: Logistic Regression, Random Forest, XGBoost  
   - Metrics: Precision, Recall, F1, AUC-ROC  
   - Business-focused evaluation (catching fraud without over-flagging)

5. **Deployment (Optional)**  
   - Streamlit dashboard to simulate real-time predictions

---
## 📂 Folder Structure
```
credit-card-fraud-detection/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_preprocessing_modeling.ipynb
│   └── 03_model_evaluation.ipynb
├── models/
│   └── saved_model.pkl (optional)
├── visuals/
│   └── feature_importance.png
├── streamlit_app/
│   └── fraud_detector.py (optional)
└── README.md
```
---

## 📬 Let’s Connect

📫 I’m **Olanrewaju Oyenekan**, actively seeking **Data Analyst / Junior Data Scientist roles (UK or remote)**  
🔗 More projects: [github.com/Larry0615](https://github.com/Larry0615)

---


