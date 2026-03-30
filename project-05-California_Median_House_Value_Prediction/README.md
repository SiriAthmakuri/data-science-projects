# California House Price Prediction

## Objective
Predict the median house value in California using various features such as income, population, and location.  
This is a **regression problem**.

## Dataset
- Total entries: 20,640  
- Columns: 10  
  1. `longitude` & `latitude` – Geographical coordinates  
  2. `housing_median_age` – Age of the housing units  
  3. `total_rooms` & `total_bedrooms` – Counts of rooms and bedrooms per location  
  4. `population` – Population of each area  
  5. `households` – Number of households in each area  
  6. `median_income` – Median income in each area  
  7. `ocean_proximity` – Categorical data indicating proximity to the ocean  
  8. `median_house_value` – Target variable (median value of houses)  

**Note:** The column `total_bedrooms` has missing values that need handling.

---

## Steps / Workflow

### 1. Data Preprocessing
- Handle missing values in `total_bedrooms` (impute with median or mean)  
- Encode `ocean_proximity` using one-hot encoding  
- Scale features like `total_rooms` and `median_income` for better model performance  

### 2. Exploratory Data Analysis (EDA)
- Correlation analysis to identify strong predictors  
- Feature engineering: `rooms_per_household`, `population_per_household`  
- Data visualization to explore trends and relationships with `median_house_value`  

### 3. Model Selection
- Linear Regression (baseline model)  
- Decision Tree Regression (captures non-linear patterns)  
- Random Forest / Gradient Boosting (ensemble methods for higher accuracy)  

### 4. Model Training & Evaluation
- Split dataset: 80% training, 20% testing  
- Train models on training set  
- Evaluate using:  
  - Mean Absolute Error (MAE)  
  - Mean Squared Error (MSE)  
  - R² Score  

### 5. Hyperparameter Tuning
- Apply Grid Search or Randomized Search with cross-validation  
- Optimize parameters for Random Forest or Gradient Boosting models  

### 6. Model Interpretation
- Feature importance plots (for tree-based models)  
- Coefficients (for linear models)  
- Insights on which features most influence `median_house_value`  

---

## Tools & Libraries
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## Usage
Open `2.california_median_house_value_prediction.ipynb` to explore the analysis, models, and visualizations step-by-step.

---

## Author
**Siri Athmakuri**  
Computer Science Engineering Student  
Aspiring Data Scientist  

GitHub: [https://github.com/SiriAthmakuri](https://github.com/SiriAthmakuri)  
LinkedIn: (Add your LinkedIn profile link)
