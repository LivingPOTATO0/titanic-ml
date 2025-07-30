# Titanic - Machine Learning from Disaster 🚢  

This project is my first Kaggle competition and my first machine learning project uploaded to GitHub.  
It predicts passenger survival from the Titanic dataset using various preprocessing techniques, supervised learning algorithms, and model evaluation methods.  

---

## 📂 Dataset  
- Competition link: [Kaggle - Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic)  
- Data files:  
  - `train.csv` → Training data with survival labels  
  - `test.csv` → Test data without labels  
  - `gender_submission.csv` → Example submission format  

---

## 🛠️ Approach  

### **1. Data Preprocessing**  
- Handling missing values (Age, Embarked, Fare)  
- Encoding categorical variables (`Sex`, `Embarked`, `Pclass`)  
- Feature engineering:  
  - `Title` (from `Name`)  
  - `FamilySize = SibSp + Parch + 1`  
  - `IsAlone = 1 if FamilySize == 1 else 0`  

### **2. Models Used**    
- Tree-based models: Random Forest  
- Gradient boosting: XGBoost (tuned)  

### **3. Model Evaluation**  
- Train/validation split using Stratified K-Fold  
- Metrics: Accuracy (Kaggle), F1-score, ROC-AUC (locally)  

---

## 📈 Results  

- **Best Kaggle Public Leaderboard Score:** `0.76`
- **Best model:** `RandomForest`  

---

## 🔗 Google Colab  

You can open and run this notebook in Colab here:  
[![Open In Colab](https://colab.research.google.com/drive/1thPY_wgoJAP1hNJwaCRLuWayy7_y_03L?usp=sharing)

---

## 📂 Repository Structure  
titanic-ml/
├── titanic-ml.ipynb # Final notebook
├── submission.csv # Best submission file
└── README.md # Project description (this file)


Author: Meet Virani

