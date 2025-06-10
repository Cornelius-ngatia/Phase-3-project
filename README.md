# Predictive Modeling for Mental Health Risks in Tech Companies.
- Using data-driven insights to identify and support at-risk employees
### Introduction
- Mental health challenges are prevalent in tech companies but often remain undetected. This project develops a predictive model using demographic and job-related data to classify employees as at risk or not at risk. The goal is to enable early intervention, enhance workplace wellness programs, and improve employee well-being.
### Business Objectives
- Early Identification – Predict employees at risk of mental health challenges.
- Key Risk Factors – Identify primary contributors, such as work stress (work_interfere) and family history.
- Proactive Intervention – Support HR teams in designing data-backed wellness strategies.
### Dataset
- Source: Survey data on workplace mental health('survey_csv)
- Size: 1,259 records, 24 features
- Target Variable: Treatment (Has the employee sought mental health treatment?)
- Key features: Treatment(Has the employee sought mental health treatment?)
### tech Stack & Libraries
- import pandas as pd 
- import numpy as np 
- import matplotlib.pyplot as plt
- import seaborn as sns
- from scipy import stats
- from sklearn.model_selection import train_test_split
- from sklearn.preprocessing import StandardScaler, LabelEncoder,MinMaxScaler
- from sklearn.linear_model import LogisticRegression
- from sklearn.tree import DecisionTreeClassifier
- from sklearn import metrics
- from sklearn.metrics import accuracy_score, mean_squared_error, precision_recall_curve
- from sklearn.model_selection import cross_val_score
- from sklearn.ensemble import RandomForestClassifier
- from sklearn.model_selection import GridSearchCV
- %matplotlib inline
### Model selection
-  Decision Tree – Easy interpretability for feature analysis
-  Logistic Regression – Probability-based classification for risk assessment
- SMOTE applied - Addressing class imbalance to ensure high recall
### Model performance
- Best Accuracy: 81% (Logistic Regression)
- Recall for "At Risk" Employees: 89% (Ensuring high-risk individuals are not overlooked)
- Feature Importance: Work stress (work_interfere) and family history
### Visualizations
- ![Alt Text](https://github.com/Cornelius-ngatia/Phase-3-project/blob/main/Images/Screenshot%202025-06-10%20114001.png)
- ![Alt Text](https://github.com/Cornelius-ngatia/Phase-3-project/blob/main/Images/Screenshot%202025-06-10%20114352.png)
- ![Alt Text](https://github.com/Cornelius-ngatia/Phase-3-project/blob/main/Images/Screenshot%202025-06-10%20115106.png)
