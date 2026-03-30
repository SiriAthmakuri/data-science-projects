# Bank Marketing Deposit Prediction

## Objective
Predict whether a client will subscribe to a **term deposit** using the bank’s marketing dataset.  
This is a **binary classification problem** in the finance/marketing domain.

---

## Dataset
- **Entries:** 11,162  
- **Columns:** 17 (10 categorical, 7 numerical)  
- **Target column:** `deposit` (Yes/No)

### Column Overview
- **Numerical:** age, balance, day, duration, campaign, pdays, previous  
- **Categorical:** job, marital, education, default, housing, loan, contact, month, poutcome, deposit  
- **Target Distribution:**  
  - No: 5,873 instances  
  - Yes: 5,289 instances

---

## Steps / Workflow

### 1. Data Preprocessing
- Handle missing or "unknown" entries in categorical features (e.g., contact, poutcome)  
- Encode categorical variables using one-hot encoding (nominal) or label encoding (binary)  
- Scale numerical features (balance, duration, etc.) using StandardScaler or MinMaxScaler  

### 2. Exploratory Data Analysis (EDA)
- Analyze target distribution to detect class imbalance  
- Correlation analysis to identify relationships among numerical features  
- Univariate and bivariate visualization to study influence of features like balance and duration  

### 3. Feature Engineering
- Create interaction features (e.g., education × job, balance × duration)  
- Transform skewed variables using logarithmic scaling or normalization  
- Feature selection based on correlation and importance metrics  

### 4. Model Selection
Binary classification models tested:
- Logistic Regression (baseline)  
- Decision Trees & Random Forests (capture non-linear relationships)  
- Gradient Boosting (XGBoost) for improved predictive accuracy  
- Support Vector Machine (SVM) for complex decision boundaries  

**Evaluation Metrics:** Accuracy, Precision, Recall, F1 Score, ROC-AUC  

### 5. Model Training & Evaluation
- Train-test split: 70-30 or 80-20  
- K-fold cross-validation for robust evaluation  
- Hyperparameter tuning using Grid Search or Random Search  
- Compare models and select the best-performing one  

### 6. Results & Interpretation
- Feature importance analysis (for tree-based models)  
- Identify key predictors of deposit subscriptions, such as call duration, account balance, and previous campaign outcome  

---

## Conclusion
- This workflow enables accurate prediction of deposit responses  
- Insights can inform targeted marketing strategies  
- Further improvement can include more feature engineering or external data validation  

---

## Tools & Libraries
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## Usage
Open `1_Bank_Marketing_Deposit_Prediction.ipynb` to explore preprocessing, analysis, model training, and evaluation step-by-step.

---

## Author
**Siri Athmakuri**  
Computer Science Engineering Student  
Aspiring Data Scientist  

GitHub: [https://github.com/SiriAthmakuri](https://github.com/SiriAthmakuri)  
LinkedIn: (www.linkedin.com/in/athmakuri-siri-20692a258)
