# 🌍 Air Quality Analysis with Python & Machine Learning

## 📌 Project Overview

This project analyzes air quality sensor data using Python and machine learning techniques.

The main objective is to explore relationships between different air-quality variables and develop a machine learning model to predict **CO (Carbon Monoxide) concentration**.

The project includes data preprocessing, exploratory data analysis, correlation analysis, visualization, machine learning model development, model evaluation, and feature-importance analysis.

---

## 🎯 Objectives

- Analyze air-quality sensor measurements
- Clean and preprocess the dataset
- Explore relationships between air-quality variables
- Visualize correlations using a heatmap
- Predict CO concentration using machine learning
- Compare Linear Regression and Random Forest models
- Identify the most important features for CO prediction
- Evaluate model performance using MAE, RMSE, and R²

---

## 🛠️ Technologies & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab
- GitHub

---

## 📊 Dataset

The project uses the **UCI Air Quality Dataset**.

The dataset contains air-quality sensor measurements collected over time.

Important variables include:

- CO(GT) – Carbon Monoxide
- PT08.S1(CO) – CO sensor response
- C6H6(GT) – Benzene concentration
- PT08.S2(NMHC) – NMHC sensor response
- NOx(GT) – Nitrogen Oxides
- PT08.S3(NOx) – NOx sensor response
- NO2(GT) – Nitrogen Dioxide
- PT08.S4(NO2) – NO2 sensor response
- PT08.S5(O3) – Ozone sensor response
- T – Temperature
- RH – Relative Humidity

---

## 🔍 Data Analysis

The project performs:

1. Dataset loading
2. Data inspection
3. Data cleaning
4. Missing-value handling
5. Data type conversion
6. Exploratory data analysis
7. Correlation analysis
8. Data visualization

---

## 📈 Correlation Analysis

A correlation heatmap was created to investigate relationships between the air-quality variables.

The analysis shows strong relationships between several sensor variables and CO concentration.

For example:

- CO(GT) and C6H6(GT) show a strong positive correlation.
- CO(GT) and PT08.S2(NMHC) show a strong relationship.
- NOx(GT) also contributes to CO prediction.
- PT08.S3(NOx) shows a strong negative relationship with several variables.

---

## 🤖 Machine Learning Models

Two machine learning models were tested:

### 1. Linear Regression

Linear Regression was used as a baseline model.

### 2. Random Forest

Random Forest was used as a non-linear machine learning model to improve prediction performance.

---

## 📊 Model Performance

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 0.3072 | 0.4797 | 0.8895 |
| Random Forest | **0.2470** | **0.3948** | **0.9252** |

### 🏆 Best Model: Random Forest

The Random Forest model achieved:

- **R² = 0.9252**
- **MAE = 0.2470**
- **RMSE = 0.3948**

The higher R² and lower error values indicate that Random Forest performed better than Linear Regression for predicting CO concentration.

---

## ⭐ Feature Importance

Feature-importance analysis was performed using the Random Forest model.

The most influential features were:

1. **PT08.S2(NMHC)**
2. **C6H6(GT)**
3. **NOx(GT)**

PT08.S2(NMHC) was identified as the most important feature for predicting CO concentration.

---

## 📉 Actual vs Predicted CO

An Actual vs Predicted plot was created to evaluate the Random Forest predictions.

The predicted values generally follow the actual CO concentrations, indicating good predictive performance.

---

## 📊 Results

The analysis demonstrates that machine learning can effectively model CO concentration from air-quality sensor measurements.

Random Forest provided better predictive performance than Linear Regression.

The model achieved an R² score of **0.9252**, indicating that it explains a large proportion of the variation in the target variable.

---

## 💡 Key Findings

- Random Forest performed better than Linear Regression.
- Random Forest achieved an R² of **0.9252**.
- PT08.S2(NMHC) was the most important feature.
- C6H6(GT) and NOx(GT) were also important predictors.
- The Actual vs Predicted plot shows that predictions generally follow observed CO concentrations.
- Machine learning can be useful for analyzing air-quality sensor data.

---

## 📁 Project Structure

```text
air-quality-prediction/
│
├── README.md
├── Untitled0.ipynb
│
└── dataset/
    └── AirQualityUCI.csv
How to Run
Option 1: Google Colab

Open the Jupyter Notebook in Google Colab and run the cells sequentially.

Option 2: Local Python Environment

Install the required libraries:

pip install pandas numpy matplotlib scikit-learn

Then open:

Untitled0.ipynb

and run the notebook.

📚 Learning Outcomes

Through this project, I practiced:

Python programming
Pandas data analysis
Data cleaning
Exploratory Data Analysis (EDA)
Data visualization
Correlation analysis
Machine learning
Regression modelling
Random Forest
Model evaluation
Feature importance
GitHub project documentation
👨‍💻 Author

Mohammad Sekandar Hossain

Artificial Intelligence | Environmental Science | GIS | Python | Data Analysis

⭐ Project Summary

This project demonstrates a practical application of Python and machine learning for air-quality analysis and CO concentration prediction.

The Random Forest model achieved the best performance among the tested models, with an R² of 0.9252.

