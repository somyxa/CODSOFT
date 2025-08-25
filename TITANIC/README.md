# Task 1: Titanic Survival Prediction

## 📌 Problem Statement
Use the Titanic dataset to build a machine learning model that predicts whether a passenger survived the Titanic disaster or not.  
This is a classic beginner project with readily available data.  

Dataset link: [Kaggle - Titanic Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset)

---

## 📊 Dataset Information
The dataset contains details of Titanic passengers such as:
- **Features**: Passenger Class (Pclass), Sex, Age, Fare, Cabin, Embarked, SibSp, Parch, etc.
- **Target**: `Survived` (0 = Did not survive, 1 = Survived)

---

## 🔎 Exploratory Data Analysis
- Checked for missing values and handled them:
  - Age → filled with median  
  - Embarked → filled with mode  
  - Cabin → filled with mode  
- Univariate analysis (distribution of survival, class, and gender)  
- Bivariate analysis (survival by gender, survival by passenger class)  
- Age distribution  
- Correlation heatmap for feature relationships  

---

## ⚙️ Data Preprocessing
- Engineered new feature: **FamilySize = SibSp + Parch**  
- Converted categorical variables (`Sex`, `Embarked`) into numeric form  
- Dropped irrelevant columns: `Name`, `Ticket`, `Cabin`  
- Standard scaling applied for Logistic Regression  

---

## 🤖 Model Training
Two classification models were applied:
1. **Logistic Regression** (on scaled features)  
2. **Random Forest Classifier** (on unscaled features)  

---

## 📈 Model Evaluation
- Metrics used: **Accuracy, Precision, Recall, F1-score, Confusion Matrix**  
- **Random Forest Classifier** performed better than Logistic Regression.  

Example Results:
- Logistic Regression: Achieved good accuracy and balanced performance.  
- Random Forest: Higher accuracy and recall in survival prediction.  

---

## 💾 Model Saving
The best-performing model (**Random Forest**) was saved as:  

titanic_best_model.pkl

## 🚀 How to Run
1. Install dependencies:  
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn joblib
