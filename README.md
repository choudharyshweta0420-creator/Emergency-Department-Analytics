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

---

## ANOVA Analysis

A one-way ANOVA test was performed to compare average length of stay across different triage severity levels.

### Result:

