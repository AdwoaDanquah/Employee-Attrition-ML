#  Employee Attrition Prediction (IBM HR Analytics)

This project explores and predicts **employee attrition**; identifying whether an employee is likely to leave or stay, using the **IBM HR Analytics dataset**.  
The analysis includes data cleaning, encoding, and a **Logistic Regression** model built with Python in Jupyter Notebook.  
The goal is to understand which factors contribute most to employee turnover and improve recall on the minority class (employees who left).

---

## Project Overview
Many organizations struggle with retaining valuable employees. This project uses real HR data to build a model that can help identify at-risk employees early.

**Main objectives:**
1. Clean and preprocess HR data for analysis.  
2. Build a classification model to predict employee attrition.  
3. Interpret model results and identify key drivers of attrition.  

---

## Tools & Libraries
- **Python 3**
- **Pandas**, **NumPy**
- **Scikit-learn**
- **Matplotlib**

---

##  Methodology
1. **Data Cleaning**  
   - Removed constant/irrelevant columns (`EmployeeCount`, `Over18`, `StandardHours`, `EmployeeNumber`).
   - Encoded the target variable `Attrition` (`Yes` = 1, `No` = 0).
   - Converted categorical variables using `pd.get_dummies()`.

2. **Data Splitting**  
   - Split the data into 80% training and 20% testing using `train_test_split()`.

3. **Modeling (Logistic Regression)**  
   - Implemented `LogisticRegression()` with:
     - `max_iter=5000` for convergence
     - `class_weight='balanced'` to address class imbalance  
   - Evaluated the model using Accuracy, Precision, Recall, and F1 Score.

4. **Visualization**  
   - Created a Confusion Matrix and ROC Curve to interpret model performance.  
   - Examined feature coefficients to identify which attributes most influence attrition.

---

## Model Performance
| Metric | Score |
| **Accuracy** | 0.75 |
| **Precision** | 0.35 |
| **Recall** | 0.64 |
| **F1 Score** | 0.45 |

The balanced Logistic Regression model significantly improved **recall** (from ~0.17 to 0.64), meaning it caught far more true attrition cases while maintaining reasonable precision.

---

## Key Insights
- **OverTime**, **MonthlyIncome**, and **JobSatisfaction** were among the top predictors of attrition.  
- Employees who work overtime or earn lower salaries are more likely to leave.  
- Balancing the classes was critical to detect more true attrition cases.  

---

## Future Improvements
- Test other models (e.g., **Random Forest**, **XGBoost**) for better recall and interpretability.    
- Build a **Tableau dashboard** to visualize employee risk in real time.  

---

## Tech Stack
**Language:** Python  
**Environment:** Jupyter Notebook  
**Libraries:** pandas, numpy, scikit-learn, matplotlib  

---

##  Author
**Stephanie A. Danquah**  
University at Albany – Data Science Master's student
 Adanquah@albany.edu 
 linkedin.com/in/stephanie-danquah-9a5435374/

---


