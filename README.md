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

The dataset consists of three files:

- `train.csv`: Training data with survival labels.
- `test.csv`: Test data used for submission.
- `gender_submission.csv`: A sample submission file provided by Kaggle.

---

## 🧹 Data Preprocessing

The following steps were applied to prepare the data:

- Dropped unused columns: `PassengerId`, `Name`, `Ticket`, `Cabin`
- Filled missing values:
  - `Age`: Replaced with median
  - `Embarked`: Filled with the mode ('S')
  - `Fare`: Filled with median (for test set)
- Applied **One-Hot Encoding** to:
  - `Sex` (converted to binary)
  - `Embarked` (created dummy variables)

---

## 🤖 Model

- **Algorithm**: Random Forest Classifier (from `sklearn.ensemble`)
- **Train/Test Split**: 80% train, 20% validation (for local evaluation)
- **Features Used**:
  - `Pclass`
  - `Sex`
  - `Age`
  - `SibSp`
  - `Parch`
  - `Fare`
  - `Embarked` (dummy variables)

---

## 📈 Submission Result

- Predictions were saved in `submission.csv`
- Submitted via Kaggle
- **Public Score**: `0.76076` (Version 1)

---

## 🚀 Next Steps / To Do

- Apply feature scaling (e.g., StandardScaler)
- Experiment with other models (Logistic Regression, XGBoost, SVM)
- Use `GridSearchCV` for hyperparameter tuning
- Perform feature importance analysis

---

## 🔗 Useful Links

- 📓 Kaggle Notebook: [Titanic - Random Forest v1](https://www.kaggle.com/code/busradeveci/titanic-randomforest-v1)
- 📁 Competition Page: [Kaggle Titanic](https://www.kaggle.com/competitions/titanic)

---

## 🧑‍💻 Author

**Büşra Deveci**  
Contact: [GitHub](https://github.com/busradeveci) | [Kaggle](https://www.kaggle.com/busradeveci)

