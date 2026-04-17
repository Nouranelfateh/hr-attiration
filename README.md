# hr-attiration
## Overview

An end-to-end HR analytics project that analyzes and predicts employee attrition using the IBM HR Employee Attrition dataset. The project combines exploratory data analysis, feature engineering, and machine learning classification in Python — then visualizes findings through a 4-page interactive Power BI dashboard.

## Dataset

1,470

Employees

35

Features

16.12%

Attrition rate

237

Left employees

Source: IBM HR Analytics Employee Attrition & Performance (Kaggle)

## Project workflow

1
Data cleaning & EDA

Dropped constant columns (EmployeeCount, Over18, StandardHours). Detected and treated outliers via IQR Winsorization across 10 features. Verified zero missing values and duplicates.

2
Feature engineering

Created 5 new features: IncomePerYear, TenureRatio, SatisfactionScore, IncomeToJobLevel, AgeSatisfaction. Label-encoded all categorical variables.

3
Class balancing & modeling

Oversampled minority class (Yes = 237 → 1,233) to balance dataset. Scaled features with MinMaxScaler. Trained 4 classifiers: Logistic Regression, Decision Tree, Random Forest, SVM.

4
Power BI dashboard

Built a 4-page dashboard with Attrition Analysis, Attrition Analysis 2, Key Influencers, and Decomposition Tree — with slicers for Department, Gender, JobRole, YearsAtCompany, and WorkLifeBalance.

## Model results

Model
Accuracy
Status
Random Forest ⭐
98.38%
Target met
SVM
91.90%
Target met
Decision Tree
80.16%
Below target
Logistic Regression
76.72%
Below target
Target accuracy: 85%  ·  Linear Regression (income prediction): R² = 0.9811, RMSE = $582.93
## Key insights

›
Overtime doubles attrition risk — employees who work overtime leave at a 30.5% rate vs. 10.4% for those who don't.

›
Employees who left earned significantly less — lower monthly income is a strong predictor of attrition.

›
First 1–2 years are critical — highest attrition occurs in early tenure, making onboarding a key retention lever.

›
Single employees have the highest attrition — 50.63% of those who left were single vs. 35.44% married and 13.92% divorced.

›
Research & Development has the highest total attrition by department count, though Sales has a higher rate relative to its size.

›
Younger employees (20–35) show disproportionately higher attrition, suggesting early-career retention programs are needed.

## Dashboard pages (Power BI)
1. Attrition Analysis

KPI cards · attrition by department · attrition by distance from home · attrition by years at company · marital status donut chart.

2. Attrition Analysis 2

Attrition by gender · overtime vs. attrition stacked bar · income vs. years scatter · job satisfaction donut.

3. Key Influencers

Power BI AI visual that automatically identifies the top factors driving attrition.

4. Decomposition Tree

Interactive tree for drilling into attrition breakdown across any combination of dimensions.

## Tech stack

Python — Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

ML models — Logistic Regression, Decision Tree, Random Forest, SVM, Linear Regression

Preprocessing — MinMaxScaler, LabelEncoder, oversampling (resample)

Power BI — DAX measures, Power Query, Key Influencers, Decomposition Tree

<img width="885" height="581" alt="image" src="https://github.com/user-attachments/assets/b87b1314-6009-48a3-9c25-69dd563a37f8" />
<img width="877" height="576" alt="image" src="https://github.com/user-attachments/assets/7b9eeb27-8151-4214-9e3a-56faf3ceb51e" />
<img width="877" height="577" alt="image" src="https://github.com/user-attachments/assets/d0aa6c87-ab07-489f-92f7-3a8a40356339" />
<img width="882" height="578" alt="image" src="https://github.com/user-attachments/assets/db4480fd-e7c8-499d-9d22-e9fa6a25b2cb" />



