# 🚨 Fraud Detection Machine Learning Project

## 🔍 Overview  
This project develops a **Machine Learning-based fraud detection system** to identify potentially fraudulent financial transactions. We use **Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, and XGBoost** for data analysis, preprocessing, feature engineering, model training, evaluation, and threshold optimization.

## 📊 Dataset  
The dataset contains **6,362,620 financial transactions** with features related to transaction type, amount, account balances, and fraud labels.

- **6,354,407** non-fraudulent transactions
- **8,213** fraudulent transactions
- Fraud rate: approximately **0.129%**

## 📌 Key Analysis & Findings  

### 1️⃣ Transaction Amount Analysis  
📌 Transaction amounts were analyzed using different value ranges to understand how fraud rates change with transaction value.  

![Transaction Amount Analysis](/transaction_amount.png)

### 2️⃣ Fraud Rate by Transaction Type  
📌 This analysis compares fraud rates across different **transaction types** and identifies transaction categories associated with fraudulent activity.  

![Fraud by Transaction Type](/fraud_by_type.png)

### 3️⃣ Fraud Rate by Hour  
📌 Transaction timing was analyzed by extracting the approximate **hour from the transaction step**. The analysis shows variation in fraud rates across different time periods.  

![Fraud Rate by Hour](/fraud_by_hour.png)

### 4️⃣ Correlation Heatmap  
📌 This heatmap shows the relationships between transaction amount and account balance features. Strong correlations between balance features motivated additional feature engineering.  

![Correlation Heatmap](/correlation_heatmap.png)

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
