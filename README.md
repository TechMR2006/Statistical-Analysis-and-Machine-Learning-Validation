# 📊 Time Series Data Analysis and Forecasting  
## 🧠 Task 5 – Machine Learning Forecasting Project  

---

## 📌 Project Overview

This project performs **Time Series Data Analysis and Forecasting** using a real-world inspired dataset:

**Apple Global Sales Dataset**

The objective is to analyze historical sales revenue over time and build a forecasting model to predict future revenue using Machine Learning techniques.

---

## 🎯 Project Covers

- Time series preprocessing  
- Missing value handling  
- Trend and seasonal analysis  
- Rolling statistics  
- Feature engineering  
- Forecasting using Linear Regression  
- Model evaluation using RMSE and MAE  

---

## 📂 Dataset Description

**Dataset Name:** `apple_global_sales_dataset.csv`

The dataset contains transaction-level Apple product sales across different regions and dates.

### 🔑 Important Columns

- `sale_date` → Date of sale  
- `revenue_usd` → Revenue generated from each sale  

Since the dataset is transactional, it was aggregated to calculate:

> **Total Daily Revenue**

This aggregation created a proper time series dataset suitable for forecasting.

---

## ⚙️ Project Workflow

---

### 1️⃣ Data Loading & Time Handling

- Loaded dataset using **Pandas**
- Converted `sale_date` to datetime format
- Aggregated revenue by date
- Set date as index
- Sorted data chronologically

✔ Result: Clean and properly indexed time series dataset.

---

### 2️⃣ Missing Value Handling

- Checked for missing values
- Applied **Linear Interpolation** to handle missing revenue values

#### ✅ Justification

Linear interpolation:

- Preserves time continuity  
- Maintains numeric structure  
- Is appropriate for time series forecasting  

---

### 3️⃣ Exploratory Time Series Analysis

A time series line plot was created to visualize:

- Overall revenue trend  
- Short-term fluctuations  
- General revenue pattern over time  

#### 📌 Observations

- Revenue shows variation over time  
- Short-term fluctuations are visible  
- A long-term trend can be observed  

---

### 4️⃣ Rolling Statistics

Calculated:

- `7-day rolling average`
- `30-day rolling average`

#### 🎯 Purpose

- 7-day average smooths short-term noise  
- 30-day average highlights long-term trend  

Rolling statistics help in understanding smoothing effects and trend direction.

---

### 5️⃣ Seasonal Decomposition

Performed **Additive Seasonal Decomposition** to separate:

- Trend component  
- Seasonal component  
- Residual component  

#### 🔍 Why Decomposition?

It helps to:

- Identify repeating patterns  
- Understand underlying trends  
- Analyze irregular fluctuations  

---

### 6️⃣ Feature Engineering

Created lag features to help the model learn from historical values:

- `lag_1` → Previous day revenue (t − 1)  
- `lag_7` → Previous week revenue (t − 7)  

#### 📌 Why Lag Features?

Lag features allow the model to:

- Capture temporal dependency  
- Learn patterns from past values  
- Improve forecasting performance  

---

## 🤖 Model Building

### Model Used:
**Linear Regression**

### Steps:

1. Train-test split  
2. Fit model on training data  
3. Predict future revenue  
4. Evaluate performance  

---

## 📊 Model Evaluation Metrics

The model was evaluated using:

- **MAE (Mean Absolute Error)**  
- **RMSE (Root Mean Squared Error)**  

### ✔ Why These Metrics?

- MAE measures average absolute prediction error  
- RMSE penalizes large errors more heavily  

Lower values indicate better forecasting performance.

---

## 🛠 Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- Statsmodels  

---

## 🚀 How to Run the Project

### 1️⃣ Install Dependencies

```bash
pip install pandas numpy matplotlib scikit-learn statsmodels
