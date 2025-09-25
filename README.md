# Decision-Tree--Credit-Risk-Scoring-Model-Loan-Default-
![alt text](<Credit Risk Scoring Model (Loan Default).jpg>)

# 🏦 Credit Risk Scoring Model (Loan Default)

##  Business Context
DRS Bank has recently experienced a rise in **loan defaults**, leading to higher levels of **Non-Performing Assets (NPAs)**. To strengthen its loan approval process, the Chief Risk Officer initiated a project to develop a data-driven framework that minimizes default risk.

The goal: **reduce loan defaults by predicting default likelihood before approval**.

---

##  Objective
1. **Predict Loan Delinquency** – Build a machine learning model to classify whether a customer is likely to default.  
2. **Identify Key Risk Drivers** – Understand which borrower attributes (e.g., FICO, loan purpose, home ownership) drive delinquency.  
3. **Support Loan Approval** – Provide a data-driven approach to minimize NPAs and improve portfolio quality.  

---

## Dataset  
- **Size**: 10,000+ loan applications  
- **Features**:
  - `isDelinquent`: Target variable (1 = Yes, 0 = No)  
  - `term`: Loan term in months  
  - `gender`: Borrower’s gender  
  - `age`: Borrower’s age  
  - `purpose`: Loan purpose (education, car, personal, etc.)  
  - `home_ownership`: Borrower’s home ownership status  
  - `FICO`: Bureau credit score of the borrower  

---

## Approach
1. **Data Understanding & Cleaning**
   - Removed duplicates and handled categorical encoding.  
   - Verified ranges of numeric variables (e.g., FICO, age).  

2. **Exploratory Data Analysis (EDA)**
   - Distribution of FICO, age, and loan purpose.  
   - Identified high-risk groups based on FICO and purpose.  

3. **Model Development**
   - Trained **Decision Tree, Logistic Regression, and XGBoost** classifiers.  
   - Handled class imbalance and tuned hyperparameters for best performance.  

4. **Model Evaluation**
   - Compared models on Accuracy, Precision, Recall, F1-score, and ROC-AUC.  
   - Selected the best-performing model for deployment.  

---

## Results
- **Best Model:** XGBoost Classifier  
- **Performance Metrics:**
  - Accuracy: 0.91  
  - Precision: 0.88  
  - Recall: 0.85  
  - F1-Score: 0.86  
- **Key Risk Drivers Identified:**
  - FICO Score (strongest predictor of delinquency)  
  - Loan Purpose (personal loans showed higher default risk)  
  - Home Ownership (renters more likely to default than owners)  

---

## Business Impact
- Provides a **data-driven loan approval framework** for minimizing NPAs.  
- Helps DRS Bank **approve safer loans**, improving profitability and risk control.  
- Enables the Risk team to **set policy thresholds** (e.g., minimum FICO score, high-risk purposes).  

---

## Tech Stack
- **Language**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost  
- **Techniques**: Classification Models, Feature Importance, Hyperparameter Tuning, ROC-AUC Evaluation  

---


