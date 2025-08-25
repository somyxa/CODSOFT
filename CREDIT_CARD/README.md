# Credit Card Fraud Detection

## 📌 Problem Statement
Build a machine learning model to identify fraudulent credit card transactions.  
The dataset is highly imbalanced, so special care is taken to handle class imbalance using **SMOTE**.  

## 📊 Dataset
- Source: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
- Transactions are labeled as:
  - `0` → Genuine
  - `1` → Fraudulent  

## ⚙️ Steps Performed
1. **Data Loading & Exploration**
   - Loaded dataset and checked distribution of fraudulent vs. genuine transactions.  
   - Visualized imbalance in target classes.  

2. **Preprocessing**
   - Split data into **train** and **test** sets.  
   - Scaled features using `StandardScaler`.  
   - Handled class imbalance using **SMOTE**.  

3. **Model Training**
   - Logistic Regression  
   - Random Forest Classifier  

4. **Evaluation**
   - Accuracy  
   - Precision, Recall, F1-score  
   - Confusion Matrix  

## 📈 Results
- Logistic Regression and Random Forest were trained.  
- Metrics used: Accuracy, Precision, Recall, F1-Score.  
- Random Forest provided better overall performance.  

## 🛠️ Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Imbalanced-learn (SMOTE)  

## 📂 Project Structure
