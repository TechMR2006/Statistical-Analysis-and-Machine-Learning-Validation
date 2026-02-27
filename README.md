# Statistical-Analysis-and-Machine-Learning-Validation
📊 Statistical Analysis & Machine Learning Validation
Superstore Sales Dataset Project
📌 Project Overview

This project performs Statistical Analysis and Machine Learning Validation on the Superstore Sales Dataset using Python.
The goal of this project is to:
Perform exploratory data analysis (EDA)
Handle missing values
Conduct hypothesis testing
Detect outliers
Apply feature scaling
Train and evaluate a Machine Learning model
Generate visualizations
Create an automated HTML statistical report



📁 project-folder
│
├── Superstore sales dataset.csv
├── analysis.py
├── statistical_report.html
├── README.md
└── 📁 visualizations
    ├── scatter_plot.png
    ├── distribution_plot.png
    ├── boxplot.png
    ├── heatmap.png
    ├── outlier_plot.png
    └── actual_vs_predicted.png


⚙️ Technologies Used:
Python
Pandas
NumPy
Matplotlib
Seaborn
SciPy
Scikit-learn

🔍 Project Workflow
1️⃣ Data Loading
Loads Superstore sales dataset.csv
Cleans column names

2️⃣ Data Preprocessing

Identifies numerical and categorical columns
Handles missing values
Numeric → filled with mean
Categorical → filled with "Unknown"

3️⃣ Descriptive Statistics

Mean
Median
Standard Deviation
Variance
Min & Max
Summary statistics table

4️⃣ Correlation Analysis
Correlation matrix
Heatmap visualization

5️⃣ Hypothesis Testing (T-Test)

Compares Sales between two Categories
Outputs:
T-statistic
P-value

6️⃣ Outlier Detection

IQR Method
Z-Score Method

7️⃣ Feature Scaling

StandardScaler applied to numerical features

8️⃣ Machine Learning Model
Train-Test Split (80-20)
Linear Regression Model
Prediction on test data

9️⃣ Model Evaluation
R² Score
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
    
