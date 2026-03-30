# Breast Cancer Diagnosis Prediction

## Objective
Predict whether a tumor is **benign or malignant** using patient diagnostic data.  
This is a **binary classification problem** in healthcare.

## Dataset
- Target column: `diagnosis` (categorical)  
- Numerical features: Age, test results, measurements, and scores relevant to diagnosis  
- Categorical features: Demographic or health indicators  

**Note:** Missing values were handled by median/mode imputation or row removal as appropriate.

---

## Steps / Workflow

### 1. Data Preprocessing
- Handle missing values  
- Encode categorical variables using one-hot encoding or label encoding  
- Standardize numerical features for consistent scaling  

### 2. Exploratory Data Analysis (EDA)
- Check distribution of diagnosis classes (handle imbalance if needed)  
- Analyze numerical feature distributions (histograms, box plots)  
- Create correlation matrix to identify features strongly related to diagnosis  

### 3. Model Selection & Training
Tested several algorithms for classification:  
- **Logistic Regression** – Baseline interpretable model  
- **Decision Tree & Random Forest** – Handle non-linear relationships and interactions; Random Forest reduces overfitting  
- **Support Vector Machine (SVM)** – Effective in high-dimensional spaces; tested with various kernels  

Evaluation method: K-fold cross-validation for robust performance estimation.

### 4. Model Evaluation & Metrics
- **Accuracy** – Overall correctness  
- **Precision & Recall** – Important for healthcare scenarios where false positives or negatives have different costs  
- **F1 Score** – Balanced metric for imbalanced data  
- **ROC-AUC Score** – Measures the model’s ability to distinguish between classes  

### 5. Key Findings
- Identified features with strong predictive power for diagnosis  
- Random Forest often provided the best performance due to its ability to capture non-linear patterns  

### 6. Conclusion
- Multiple factors significantly influence diagnosis predictions  
- Selected model can support clinical decisions, though further validation on external datasets is recommended

---

## Tools & Libraries
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## Usage
Open `1_Breast_cancer_diagnosis_Prediction.ipynb` to explore the analysis, model training, and evaluation step-by-step.

---

## Author
**Siri Athmakuri**  
Computer Science Engineering Student  
Aspiring Data Scientist  

GitHub: [https://github.com/SiriAthmakuri](https://github.com/SiriAthmakuri)  
LinkedIn: (Add your LinkedIn profile link)
