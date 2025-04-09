# Car-Price-Prediction-Regression-Modeling-Project

# 🚗 Car Price Prediction: Regression Modeling Project

## 📊 Problem Overview

A Chinese automobile company plans to enter the US market and wants to understand the key factors influencing car prices in the region. By analyzing various vehicle specifications and features, the objective is to **predict car prices** using multiple regression models.

This project helps the company:

- Identify the **most important variables** affecting price
- Gain insights into **pricing dynamics** of the American market
- Use machine learning to **guide design and business strategy**

---

## 📁 Dataset

- Source: [`CarPrice_Assignment.csv`](./CarPrice_Assignment.csv)
- Features: Engine specs, body details, brand, mileage, horsepower, etc.
- Target: `price` (continuous)

---

## ✅ Project Workflow

### 1️⃣ Data Preprocessing

- Extracted brand from `CarName`
- Dropped irrelevant or duplicate features
- Encoded categorical variables using `pd.get_dummies()`
- Scaled numerical features using `StandardScaler`

### 2️⃣ Models Implemented

- 🔹 Linear Regression
- 🌳 Decision Tree Regressor
- 🌲 Random Forest Regressor
- 🔺 Gradient Boosting Regressor
- 🌀 Support Vector Regressor (SVR)

All models were trained and evaluated using `R²`, `MAE`, and `MSE`.

### 3️⃣ Hyperparameter Tuning

GridSearchCV was applied to:

- Random Forest
- Gradient Boosting
- Decision Tree
- Ridge Regression
- SVR

### 4️⃣ Feature Importance & Interpretation

- 📌 Top features from Random Forest: `enginesize`, `curbweight`, `horsepower`, `highwaympg`
- 🔍 SHAP plots used to interpret Gradient Boosting predictions

---

## 🏆 Model Comparison

| Model                | R² Score | MAE     | MSE        |
|---------------------|----------|---------|------------|
| Random Forest        | **0.958** | ✅ Best | ✅ Best     |
| Gradient Boosting    | 0.924     | Good    | Good       |
| Decision Tree        | 0.907     | Fair    | Fair       |
| SVR                  | ❌        | Poor    | Poor       |
| Linear Regression    | ❌        | ❌      | ❌ Extreme error |

> 🔥 **Random Forest Regressor outperformed all models** with the highest R² and lowest MAE/MSE.

---

## 📈 Visual Highlights

- SHAP summary plot for interpretability
- Feature importance via Random Forest & Linear Regression coefficients
- Model performance comparison charts

---

## 📌 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/car-price-regression.git
   cd car-price-regression
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch the notebook:
   ```bash
   jupyter notebook ml-moduel-asisgnment.ipynb
   ```

---

## 🔧 Dependencies

- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`
- `shap`

---

## 📬 Author

- **Your Name**  
  📧 jacobtjoshy@gmail.com
  🌐 https://github.com/Jacob-Thomas-I21

---

## 🎓 Academic Note

This project was completed as part of a machine learning module and is intended for both academic and portfolio purposes. All models were implemented from scratch using open-source libraries and evaluated against real-world metrics.

