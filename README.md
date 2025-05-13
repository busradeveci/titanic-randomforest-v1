# Titanic - Random Forest (v1)

This repository contains my solution to the classic Kaggle competition: **Titanic - Machine Learning from Disaster**. The goal is to predict which passengers survived the Titanic shipwreck using a classification model.

---

## 📊 Overview

- **Competition**: [Titanic - Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic)
- **Model**: Random Forest Classifier
- **Public Score**: `0.76076`
- **Best Score**: `0.76076` (Version 1)

---

## 📁 Dataset

The dataset includes passenger details such as age, gender, ticket class, number of siblings/spouses aboard, and fare. These features were used to build the model.

---

## 🧹 Data Preprocessing

The following preprocessing steps were applied:

- Dropped unnecessary columns: `PassengerId`, `Name`, `Ticket`, `Cabin`
- Filled missing values:
  - `Age`: Filled with median
  - `Embarked`: Filled with mode (`'S'`)
  - `Fare`: Filled with median (only in test set)
- Converted categorical variables:
  - `Sex`: Binary mapping
  - `Embarked`: One-Hot Encoding

---

## 🤖 Model

- **Algorithm**: `RandomForestClassifier` from `sklearn.ensemble`
- **Training-Validation Split**: 80% training / 20% validation
- **Selected Features**:
  - `Pclass`
  - `Sex`
  - `Age`
  - `SibSp`
  - `Parch`
  - `Fare`
  - One-hot encoded `Embarked`

The model was trained and evaluated using basic performance metrics.

---

## 📈 Results

- Achieved a public Kaggle score of **0.76076**
- This was the first version of the model and performed well on the leaderboard.

---

## 🚀 Next Steps

Planned improvements and experiments:

- Try other models (e.g., Logistic Regression, XGBoost)
- Perform hyperparameter tuning using GridSearchCV
- Use feature importance to select or engineer better features
- Consider using cross-validation for more reliable evaluation

---

## 🔗 Resources

- 📓 Kaggle Notebook: [Titanic - Random Forest v1](https://www.kaggle.com/code/busradeveci/titanic-randomforest-v1)
- 🏆 Competition Page: [Kaggle Titanic](https://www.kaggle.com/competitions/titanic)

---

## 🧑‍💻 Author
Kaggle: [kaggle.com/busradeveci](https://www.kaggle.com/busradeveci)
