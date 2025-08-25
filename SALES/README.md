# 📊 Sales Prediction using Machine Learning

## 📌 Project Overview

This project focuses on **predicting product sales** based on advertising expenditure across different channels such as **TV, Radio, and Newspaper**. By using **machine learning models** in Python, businesses can forecast sales and make data-driven decisions to optimize advertising strategies.

The dataset contains details of advertising costs and corresponding sales, and the goal is to build regression models to accurately predict sales.

---

## 🗂️ Dataset

* Source: [Advertising Dataset (Kaggle)](https://www.kaggle.com/code/ashydv/sales-prediction-simple-linear-regression/input)
* Features:

  * **TV** – Budget spent on TV advertisements
  * **Radio** – Budget spent on Radio advertisements
  * **Newspaper** – Budget spent on Newspaper advertisements
* Target:

  * **Sales** – Product sales in units

---

## 🔍 Exploratory Data Analysis (EDA)

The dataset was analyzed to identify relationships between features and the target variable:

* Distribution plots of all features
* Pairplots to check linearity
* Correlation heatmap (TV and Radio showed strong correlation with Sales, while Newspaper was weaker)
* Scatterplots of each feature vs Sales

---

## ⚙️ Model Building

Two regression models were implemented:

1. **Linear Regression (Scaled data)**

   * Used StandardScaler for feature scaling
   * Evaluated with R², RMSE, and MAE

2. **Random Forest Regressor (Unscaled data)**

   * Ensemble model for improved accuracy
   * Compared performance with Linear Regression

---

## 📈 Results

* **Linear Regression Performance**

  * R² Score: \~0.90
  * RMSE: (printed in output)
  * MAE: (printed in output)

* **Random Forest Performance**

  * R² Score: \~0.96 (better fit)
  * RMSE: (printed in output)
  * MAE: (printed in output)

* Random Forest outperformed Linear Regression, showing the non-linear relationships in data.

---

## 📊 Visualizations

* Feature distributions
* Pairplot of features
* Correlation heatmap
* Predictions vs Actual values (for both models)
* Residual distribution (Linear Regression)

---

## 💾 Model Saving

Both models were saved for future use:

* `linear_regression_model.pkl`
* `random_forest_model.pkl`
* `scaler.pkl`

---

## 🚀 How to Run the Project

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/sales-prediction.git
   cd sales-prediction
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the script:

   ```bash
   python sales_prediction.py
   ```

4. Models will be saved automatically in the working directory.

---

🔮 Future Improvements

Use advanced regression models (XGBoost, Gradient Boosting)

Perform hyperparameter tuning for Random Forest

Deploy the model as a Flask/Django web app

Add feature importance visualization

✨ Conclusion

This project demonstrates how machine learning can be applied to real-world business problems like sales forecasting. By leveraging advertising data, companies can optimize ad spend and maximize sales potential.