
# 💳 Fraud Detection on Financial Transactions

This notebook presents a machine learning approach to detecting fraudulent financial transactions. The dataset is **highly imbalanced**, with less than 0.13% of transactions being fraudulent. The project demonstrates preprocessing, feature engineering, exploratory analysis, and modeling techniques tailored to this challenge.

---

## 📊 Problem Overview

The goal is to **classify transactions as fraudulent or legitimate**. Due to severe class imbalance, the model selection and evaluation strategies are designed to handle skewed distributions effectively.

---

## 🧰 Technologies Used

- Python 3.x
- Pandas & NumPy for data handling
- Matplotlib & Seaborn for visualizations
- Scikit-learn for preprocessing and modeling
- VIF analysis for multicollinearity
- Decision Tree & Random Forest for classification

---

## 🔍 Workflow Summary

### 1. 📥 Data Import and Exploration
- Loaded the dataset from CSV
- Checked for class imbalance
- Examined basic statistical properties

### 2. 🧹 Data Preprocessing
- Label Encoding for object columns (like `nameOrig`, `nameDest`)
- Addressed multicollinearity using **Variance Inflation Factor (VIF)**
- Dropped or combined collinear features

### 3. 📊 Visualization
- **Correlation Heatmap** to observe feature relationships
- Distribution of fraud vs legit transactions
- Bar plots for class distribution

### 4. 🧠 Model Building
- Applied:
  - **Decision Tree Classifier**
  - **Random Forest Classifier**
- Chosen due to robustness with imbalanced data
- Evaluated with accuracy, precision, recall, and F1 score

---

## ⚠️ Class Imbalance Note

> With only ~0.13% of fraudulent transactions, **accuracy alone is misleading**.
> Metrics like **recall, precision, and F1-score** are emphasized to assess performance.

---

## 📦 Project Structure

```
fraud_detection.ipynb
README_FraudDetection.md
data/
    └── transactions.csv
```

---

## 📌 Next Steps / Improvements

- Apply **SMOTE** or **under-sampling** to balance data
- Try **XGBoost** or **LightGBM**
- Deploy using Flask or Streamlit
- Integrate real-time prediction on transaction streams

---

## 👤 Author

**Yash Vinaychandra Rana**  
Graduate Student, Concordia University  
📧 yashrana240203@gmail.com  
📞 +1-438-836-5297

---

## 📄 License

This project is licensed under the MIT License.
