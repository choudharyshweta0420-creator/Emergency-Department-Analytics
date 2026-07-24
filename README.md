# Emergency Department Analytics: Predicting Hospital Admission Risk Using Statistical Analysis and Machine Learning

## Project Overview

Emergency departments face challenges such as prolonged patient length of stay (LOS), differences in outcomes across triage severity levels, and the need to identify patients who may require hospital admission early in their visit.

This project analyzes synthetic Emergency Department (ED) visit data to explore factors associated with patient flow, length of stay, and admission outcomes. Statistical analysis and machine learning techniques were applied to generate insights that can support operational planning, early risk stratification, and data-driven decision-making in healthcare settings.

---

## Business Problem

Emergency department leadership wanted to understand:

- What factors contribute to longer emergency department length of stay?
- Do patient outcomes differ across triage severity levels?
- Can patient admission risk be predicted early using available visit information?

The goal was to apply healthcare analytics methods to improve patient flow management and support clinical operations.

---

## Dataset Description

The dataset contains **400 synthetic emergency department patient visits**.

Each row represents a single ED visit and includes information related to:

### Patient Information
- Age
- Demographics

### Clinical Information
- Triage severity level
- Admission status
- Patient characteristics

### Operational Information
- Emergency department length of stay (hours)
- Number of diagnostic tests ordered

### Target Variable
- **Admitted**
  - 1 = Patient admitted to hospital
  - 0 = Patient discharged

---

## Tools and Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

---

# Project Workflow

## 1. Data Exploration

Performed initial exploration to understand:

- Dataset structure
- Number of rows and columns
- Variable types
- Data characteristics

---

## 2. Emergency Department Length of Stay Analysis

Calculated:

- Mean ED length of stay
- Median ED length of stay

The analysis helped identify the typical patient stay duration and assess potential skewness caused by extreme values.

---

## 3. Data Visualization

Created visualizations to compare:

- Length of stay between admitted and non-admitted patients

These visualizations helped identify patterns in patient flow and admission outcomes.

---

# Statistical Analysis

## Hypothesis Testing

An independent statistical test was performed to compare ED length of stay between:

- Admitted patients
- Non-admitted patients

Purpose:

To determine whether differences in LOS between groups were statistically meaningful.

## ANOVA Analysis

A one-way ANOVA test was performed to compare average length of stay across different triage severity levels.

### Result:
F-statistic: 0.1208
P-value: 0.8862


### Interpretation:

The analysis did not identify a statistically significant difference in average ED length of stay across triage severity levels.

This suggests that other factors beyond triage level may influence ED LOS.

---

# Predictive Modeling

Machine learning models were developed to predict hospital admission risk.

The following predictors were used:

- Age
- ED length of stay
- Number of diagnostic tests ordered

---

## Model 1: Logistic Regression

Logistic regression was used to predict the probability of hospital admission.

### Performance:

Accuracy:
70%


ROC-AUC:
0.65


### Interpretation:

The model demonstrated moderate ability to distinguish between admitted and non-admitted patients.

---

## Model 2: Decision Tree Classifier

Decision trees were used to capture possible non-linear relationships between patient characteristics and admission outcomes.

### Performance:

Accuracy:
61.25%


### Interpretation:

The model was easy to interpret but showed lower predictive performance compared with logistic regression.

---

## Model 3: Random Forest Classifier

A random forest model was developed using multiple decision trees to improve stability and predictive performance.

### Performance:

Accuracy:
65%


### Interpretation:

The random forest provided more stable predictions than a single decision tree but did not outperform logistic regression in this dataset.

---

# Model Performance Comparison

| Model | Accuracy |
|------|----------|
| Logistic Regression | 70% |
| Random Forest | 65% |
| Decision Tree | 61.25% |

---

# Key Findings

- Longer emergency department stays and increased diagnostic testing were associated with higher likelihood of hospital admission.
- Predictive models can support early identification of patients who may require admission.
- Logistic regression provided the strongest performance among the tested models.
- Additional clinical variables could improve prediction accuracy.

---

# Operational Impact

The insights from this analysis can help emergency department teams:

- Improve early patient risk assessment
- Allocate resources more efficiently
- Identify patients requiring closer monitoring
- Support operational planning and patient flow improvements

Predictive models should support, not replace, clinical decision-making.

---

# Limitations

This project used synthetic data, which may not represent the complexity of real-world emergency department environments.

Future improvements could include:

- Vital signs
- Laboratory results
- Diagnosis information
- Previous hospitalization history
- Physician assessments
- Social determinants of health

---

# Future Improvements

Potential enhancements include:

- Feature engineering
- Model tuning
- Cross-validation
- Fairness and bias evaluation
- Deployment using healthcare analytics dashboards

---

# Project Files
│
├── ED_Analytics_Project.ipynb
├── ED_dataset.csv
├── README.md
└── charts/
├── LOS_by_Admission.png
├── ROC_Curve.png
└── Model_Comparison.png


---

# Author- Shweta Choudhary

Healthcare Data Analytics Portfolio Project

Skills Demonstrated:

- Healthcare Data Analysis
- Statistical Testing
- Hypothesis Testing
- Machine Learning
- Predictive Modeling
- Python Programming
- Data Visualization---



