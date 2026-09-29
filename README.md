# 🚨 Fraud Detection Machine Learning Project

## 🔍 Overview  
This project develops a **Machine Learning-based fraud detection system** to identify potentially fraudulent financial transactions. We use **Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, and XGBoost** for data analysis, preprocessing, feature engineering, model training, evaluation, and threshold optimization.

## 📊 Dataset  
The dataset contains **6,362,620 financial transactions** with features related to transaction type, amount, account balances, and fraud labels.

- **6,354,407** non-fraudulent transactions
- **8,213** fraudulent transactions
- Fraud rate: approximately **0.129%**

## 💡 Key Insights  
✔ **Fraudulent transactions are highly imbalanced**, making accuracy alone insufficient for evaluating the model.

✔ **Higher-value transactions** show noticeably higher fraud rates.

✔ **Transaction type and transaction timing** provide useful signals for identifying fraudulent transactions.

✔ **Balance-related features** show strong relationships, leading to the creation of balance-difference features.

✔ **Threshold optimization** significantly improves fraud precision while maintaining high fraud recall.

## 📌 Key Analysis & Findings  

### 1️⃣ Fraud Distribution  
📌 This visualization shows the distribution of **fraudulent and non-fraudulent transactions**, highlighting the severe class imbalance in the dataset.  

![Fraud Distribution](images/fraud_distribution.png)

### 2️⃣ Transaction Amount Analysis  
📌 Transaction amounts were analyzed using different value ranges to understand how fraud rates change with transaction value.  

![Transaction Amount Analysis](images/transaction_amount.png)

### 3️⃣ Fraud Rate by Transaction Type  
📌 This analysis compares fraud rates across different **transaction types** and identifies transaction categories associated with fraudulent activity.  

![Fraud by Transaction Type](images/fraud_by_type.png)

### 4️⃣ Fraud Rate by Hour  
📌 Transaction timing was analyzed by extracting the approximate **hour from the transaction step**. The analysis shows variation in fraud rates across different time periods.  

![Fraud Rate by Hour](images/fraud_by_hour.png)

### 5️⃣ Correlation Heatmap  
📌 This heatmap shows the relationships between transaction amount and account balance features. Strong correlations between balance features motivated additional feature engineering.  

![Correlation Heatmap](images/correlation_heatmap.png)

### 6️⃣ Model Performance Comparison  
📌 **Logistic Regression, Random Forest, and XGBoost** were trained and compared using accuracy, precision, recall, and F1-score.  

![Model Performance Comparison](images/model_comparison.png)

### 7️⃣ Precision-Recall Curve  
📌 The **Precision-Recall curve** was used to optimize the classification threshold because the dataset contains a highly imbalanced fraud class.  

![Precision Recall Curve](images/precision_recall_curve.png)

### 8️⃣ Confusion Matrix  
📌 The final tuned XGBoost model achieved approximately **90% fraud recall and 33.8% fraud precision** at the optimized threshold.  

![Confusion Matrix](images/confusion_matrix.png)

## 🛠 Technologies Used  
- **Python, Pandas, NumPy** – Data manipulation and analysis  
- **Matplotlib, Seaborn** – Data visualization  
- **Scikit-learn** – Preprocessing, machine learning, and evaluation  
- **XGBoost** – Gradient boosting classification  
- **Joblib** – Model saving and serialization  

## 💡 **Key Insights**  

✔ **Fraud detection is a highly imbalanced classification problem**, with fraudulent transactions representing only about **0.129%** of the dataset.

✔ **Transaction amount, transaction type, and timing** provide useful signals for fraud detection.

✔ **Feature engineering** using balance differences helps capture changes in account balances.

✔ **XGBoost achieved 96% fraud recall and 8% precision** using the default classification threshold.

✔ **Threshold optimization increased precision to approximately 33.8% while maintaining approximately 90% fraud recall.**

## 🚀 **Why This Project Matters**  

📌 **For Financial Institutions:** Helps identify potentially fraudulent transactions using machine learning techniques.

📌 **For Fraud Analysts:** Helps prioritize suspicious transactions for further investigation.

📌 **For Data Scientists:** Demonstrates practical experience with **EDA, data preprocessing, feature engineering, imbalanced classification, model comparison, threshold optimization, and model evaluation**.

📌 **For Employers:** Demonstrates hands-on expertise in **Python, Machine Learning, XGBoost, Scikit-learn, data analysis, and visualization**.
