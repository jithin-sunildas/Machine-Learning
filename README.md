# ML_Assignment_3 - Regression 📉

## 📌 Project Overview

This project demonstrates the application of various regression techniques to the **California Housing dataset** 🏡—a real-world dataset containing features related to houses in California and their median values. The goal is to understand and compare the performance of different regression algorithms using standard evaluation metrics. 📊

## 🎯 Objective

The main objective of this assignment is to evaluate and compare several regression methods in order to **predict median house values**. The project involves:

✅ Loading and preprocessing the data.  
✅ Implementing multiple regression algorithms.  
✅ Evaluating and comparing model performance using metrics such as **Mean Squared Error (MSE)**, **Mean Absolute Error (MAE)**, and **R-squared (R²)**.  
✅ Providing clear documentation and explanations throughout the process.  

## 🏡 Dataset

We use the **California Housing dataset** available from the `sklearn` library. The dataset contains the following key features:

- **MedInc:** Median income in block group. 💰  
- **HouseAge:** Median house age in block group. 🏠  
- **AveRooms:** Average number of rooms per household. 🚪  
- **AveBedrms:** Average number of bedrooms per household. 🛏️  
- **Population:** Block group population. 👨‍👩‍👧‍👦  
- **AveOccup:** Average number of household members. 🏡  
- **Latitude:** Block group latitude. 🌍  
- **Longitude:** Block group longitude. 🗺️  
- **MedHouseVal:** Median house value (target variable). 📈  

## ⚙️ Preprocessing

### 🔧 Steps Performed:
- **Loading Data:** The dataset is fetched using `fetch_california_housing` and converted into a pandas DataFrame. 📊  
- **Missing Values:** The dataset has no missing values by default; however, we check and treat any if found. ✅  
- **Feature Scaling:** We standardize the features using `StandardScaler` to ensure they are on a comparable scale—critical for many regression algorithms. 🔬  
- **Train-Test Split:** The data is split into **training and testing sets** for model evaluation. 📚  

## 🚀 Regression Algorithms Implemented

We implement and compare the following **regression models**:

### 1️⃣ **Linear Regression**  
📏 A straightforward approach that fits a linear relationship between the features and the target.  

### 2️⃣ **Decision Tree Regressor**  
🌳 A non-linear model that partitions the feature space into regions with similar target values.  

### 3️⃣ **Random Forest Regressor**  
🌲 An ensemble of decision trees that improves prediction accuracy by averaging multiple trees.  

### 4️⃣ **Gradient Boosting Regressor**  
📉 An iterative ensemble method that builds models sequentially to reduce errors from previous models.  

### 5️⃣ **Support Vector Regressor (SVR)**  
📡 Uses support vector machines to perform regression with a specified margin of tolerance.  

Each model is evaluated using:  
📌 **Mean Squared Error (MSE)**  
📌 **Mean Absolute Error (MAE)**  
📌 **R-squared (R²) Score**  

## 📊 Model Evaluation & Comparison

The evaluation results for each model are compiled into a table, allowing easy comparison. The **best-performing model** is identified based on the highest **R² score**, and the **worst-performing model** is noted with reasons based on the evaluation metrics.  

## 🛠️ How to Run the Project

### ✅ Prerequisites
- 🐍 Python 3.x  
- 📓 Jupyter Notebook  
- 📦 Required libraries: `pandas`, `numpy`, `scikit-learn`, `seaborn`, `matplotlib`  

