# Insurance Cost Prediction using Machine Learning

Machine Learning project focused on predicting healthcare insurance costs using regression models and data-driven business analysis.

This project analyses customer health, lifestyle, demographic, and medical history data to predict insurance costs accurately. The objective is to help insurance companies improve premium pricing strategies, risk assessment, and operational decision-making using Machine Learning techniques.

---

## Project Overview

Healthcare insurance pricing requires accurate estimation of customer risk profiles. Incorrect premium pricing may lead to:
- Financial losses for insurance companies
- Unfair premium costs for customers
- Poor risk assessment
- Operational inefficiencies

This project uses Machine Learning and statistical modelling techniques to:
- Analyse factors influencing insurance costs
- Identify key health and lifestyle risk indicators
- Build predictive regression models
- Generate actionable business recommendations

---

## Business Objective

The objective of this project is to:
- Predict individual insurance costs accurately
- Identify the key factors influencing insurance premiums
- Improve insurance risk assessment strategies
- Support data-driven premium pricing decisions

---

## Dataset Information

The dataset contains:
- **25,000 customer records**
- **24 features**
- Continuous target variable:
  - `insurance_cost`

### Important Features
- Age
- BMI
- Weight
- Smoking status
- Exercise habits
- Cholesterol level
- Average glucose level
- Doctor visits
- Health checkups
- Medical history
- Insurance history

---

## Technologies & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- XGBoost
- SciPy
- Google Collab Notebook

---

## Exploratory Data Analysis (EDA)

### Key Insights

- Weight showed the strongest positive relationship with insurance cost
- Most lifestyle and demographic variables showed weak standalone correlations
- Customers with hospitalization history generally had higher insurance costs
- Engineered health-risk features improved predictive power
- BMI contained significant outliers and required treatment
- Missing values and structural inconsistencies required preprocessing

---

## Data Preprocessing

### Steps Performed
- Removed irrelevant identifier column (`applicant_id`)
- Corrected spelling inconsistencies
- Missing value treatment
- Outlier detection using:
  - IQR Method
  - Boxplots
- Winsorization for BMI outliers
- Feature scaling using StandardScaler
- One-hot encoding for categorical variables
- Train-validation-test split
- Data leakage prevention

---

## Feature Engineering

Created engineered features such as:
- `ever_hospitalized`
- `years_since_last_admission`
- `health_risk_score`

These features improved the model’s ability to capture:
- Health-risk patterns
- Hospitalization impact
- Medical severity relationships

---

## Machine Learning Models

### Baseline Model
- Linear Regression (OLS)
- VIF-based multicollinearity handling
- Backward elimination using p-values
- Assumption testing

### Advanced Models
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor
- AdaBoost Regressor

---

## Hyperparameter Tuning

Hyperparameter tuning was performed using:
- GridSearchCV
- Cross-validation techniques

### Tuned Models
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor

---

## Model Evaluation Metrics

Models were evaluated using:
- RMSE
- MAE
- R² Score
- Adjusted R²
- MAPE

---

## Final Model Selection

Multiple regression models were compared based on:
- Generalisation ability
- Prediction accuracy
- RMSE performance
- Overfitting control
- Business interpretability

The final selected model balanced:
- Strong predictive performance
- Minimal overfitting
- Better generalisation on unseen data

---

## Business Insights

### High Insurance Cost Factors
- Higher body weight
- Hospitalization history
- Frequent doctor visits
- Higher health-risk scores

### Lower Insurance Cost Factors
- Regular health checkups
- Longer insurance tenure
- Better lifestyle management patterns

---

## Business Recommendations

- Implement risk-based premium pricing strategies
- Encourage preventive healthcare and regular checkups
- Use predictive analytics for customer risk profiling
- Improve premium fairness using data-driven models
- Monitor high-risk customer segments proactively

---

## Project Structure

- `TasmiyaSana_InsuranceCostPrediction_FinalReport.pdf` — Detailed business report
- `TasmiyaSana_InsuranceCostPrediction_Notebook.ipynb` — Full implementation notebook
- `Data.csv` — Full health insurance dataset csv file
- `README.md` — Project documentation

---

## Author

Tasmiya Sana

---

## Conclusion

This project demonstrates how Machine Learning and regression modelling can help predict healthcare insurance costs accurately. By identifying important health and lifestyle risk factors, insurance companies can improve premium pricing strategies, enhance operational efficiency, and support fair risk assessment systems.
