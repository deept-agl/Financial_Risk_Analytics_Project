# 📉 Credit Risk Prediction — Financial Risk Analytics

This project focuses on predicting company default risk using financial statement data. It analyzes balance-sheet indicators, growth ratios, liquidity metrics, and cash-flow variables to identify which companies are likely to default and why.

---

## 🚀 Project Overview
The dataset contains **3,478 companies** with **67 financial variables** from the 2015–2016 period. The goal is to classify companies as **default** or **non-default** based on their financial health. The project includes:

- Outlier treatment using min–max substitution  
- Missing value handling  
- Target variable creation based on next year’s net worth  
- Univariate & bivariate analysis  
- Correlation and covariance analysis  
- Model building & evaluation  

---

## 📊 Models Used

### **1. Logistic Regression**
- Built using StatsModels  
- Variables selected using VIF and p-value filtering  
- Achieved **~83% accuracy** with a cut-off of 0.17  
- Identified key drivers of default such as:  
  - Total Debt  
  - Net Working Capital  
  - Market Capitalisation  
  - ROG Gross Block %  
  - CEPS  

### **2. Random Forest**
- Tuned using GridSearchCV  
- Very high accuracy (~98%) but signs of overfitting  

### **3. Linear Discriminant Analysis (LDA)**
- Strong performance (~91% accuracy)  
- Good alternative with balanced generalization  

---

## 📈 Key Insights
- ~11% of companies in the dataset are defaulters  
- High leverage, weak liquidity, and poor asset returns strongly signal default  
- Growth ratios (ROG variables) significantly influence risk  
- Logistic Regression offers the best balance of interpretability and performance  
- Random Forest performs well but may overfit  
- LDA performs consistently with low computational cost  

---

## 🧠 Financial Recommendations
- Monitor companies with high debt, low working capital, and declining asset growth  
- Use model insights to improve credit screening and reduce lending risk  
- Incorporate additional variables such as past loan defaults for better accuracy  

---

## 🛠️ Tech Stack
- Python  
- Pandas, NumPy  
- StatsModels, Scikit-Learn  
- Matplotlib, Seaborn  

---

⭐ *If this project helped you, feel free to star the repo!*
