# 🚗 Car Price Prediction

## 📌 Project Overview
This project aims to predict car prices based on various independent features using multiple regression models. The goal is to help a Chinese automobile company understand the factors affecting car pricing in the American market, enabling better design and marketing strategies.

## 📊 Dataset
- The dataset contains various features related to cars, including specifications, engine performance, and pricing.
- It has been sourced from market surveys and includes both numerical and categorical data.

## 🔑 Key Components
### 1️⃣ Data Preprocessing
- Load dataset and handle missing values.
- Encode categorical variables.
- Standardize numerical features.
- Split data into training and testing sets.

### 2️⃣ Model Implementation
The following regression models have been implemented:
- **📈 Linear Regression**
- **🌳 Decision Tree Regressor**
- **🌲 Random Forest Regressor**
- **🚀 Gradient Boosting Regressor**
- **🔢 Support Vector Regressor (SVR)**

### 3️⃣ Model Evaluation
Each model is evaluated based on:
- **📏 R-squared (R²)**: Measures how well the model explains variance in car prices.
- **📉 Mean Squared Error (MSE)**: Measures prediction error magnitude.
- **📊 Mean Absolute Error (MAE)**: Measures absolute difference between predicted and actual values.

### 4️⃣ Feature Importance Analysis
- Used Random Forest to identify the most influential factors affecting car prices.
- Helps in feature selection and business insights.

### 5️⃣ Hyperparameter Tuning
- Applied **🔍 GridSearchCV** to fine-tune Random Forest parameters for improved performance.

## 🏆 Results
- Models are compared using evaluation metrics.
- Feature importance analysis highlights key attributes influencing pricing.
- Best-performing model is identified based on highest R² and lowest error metrics.

## ⚙️ How to Run
1. Install dependencies: `pip install -r requirements.txt`
2. Run the Jupyter Notebook.
3. View model results and feature importance insights.

## ✍️ Author
- **[Your Name]**

## 📜 License
This project is for educational purposes and is open-source.

---
Feel free to modify this document as needed! 🚀

