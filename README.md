# 🛡️ Credit Card Fraud Detection

This project implements a **machine learning pipeline** to detect fraudulent transactions in credit card data.  
It uses the [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud) (284,807 transactions, only 492 frauds → **highly imbalanced dataset**).

---

## 📌 Project Overview
- Preprocessed and explored the dataset
- Handled class imbalance
- Trained multiple machine learning models
- Evaluated with appropriate metrics
- Suggested improvements for real-world deployment

---

## 📂 Dataset
- **File:** `creditcard.csv`
- **Features:** 30 (including PCA-transformed `V1`–`V28`, `Time`, and `Amount`)
- **Target:** `Class` (0 = Legitimate, 1 = Fraud)
- **Size:** 284,807 rows × 31 columns

---

## ⚙️ Steps in the Notebook
1. **Data Loading & Exploration**
   - Checked distributions of fraud vs non-fraud
   - Explored transaction amounts and time features

2. **Preprocessing**
   - Standardized `Amount` feature
   - Handled imbalance with techniques like undersampling / oversampling (can extend with SMOTE/ADASYN)

3. **Model Training**
   - Logistic Regression
   - Decision Tree
   - Random Forest
   - K-Nearest Neighbors
   - (extendable to XGBoost, LightGBM, Isolation Forest, Autoencoders)

4. **Evaluation**
   - Confusion Matrix
   - Classification Report
   - Accuracy Score  
   ⚠️ Note: Accuracy is misleading on imbalanced datasets → should rely on **Precision, Recall, F1, ROC-AUC, and PR-AUC**.

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/Credit_Card_Fraud_Detection.git
   cd Credit_Card_Fraud_Detection
