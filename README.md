# Titanic-Survival-Prediction

An end to end Machine Learning project built on the famous Titanic dataset to predict whether a 
passenger survived or not based on features like age, gender, class, fare, and family details.

## Project Overview

This project demonstrates the complete machine learning workflow:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Preprocessing
- Model Training
- Model Evaluation
- Model Comparison

The goal was to test multiple classification algorithms and identify the best-performing model.

---

## Dataset

Dataset: Titanic - Machine Learning from Disaster

Target Variable:

- Survived
  - 0 = Did Not Survive
  - 1 = Survived

Features:

- Pclass
- Sex
- Age
- Fare
- Embarked
- SibSp
- Parch
- Name
- Ticket
- Cabin

---

## What I Did in This Project

### 1. Data Cleaning

- Removed Cabin column due to many missing values
- Filled missing values in Age using median
- Filled missing values in Embarked using mode
- Fixed preprocessing flow to avoid data leakage

### 2. Exploratory Data Analysis (EDA)

Performed univariate and multivariate analysis using visualizations.

#### Univariate Analysis

- Survival distribution
- Passenger class distribution
- Gender distribution
- Age distribution
- Fare distribution
- Outlier detection

#### Multivariate Analysis

- Survival vs Pclass
- Survival vs Sex
- Survival vs Embarked
- Survival vs Age
- Survival vs Fare
- Correlation heatmap

### 3. Feature Engineering

Created new useful features:

- Family_size = SibSp + Parch
- family_type:
  - Alone
  - Medium
  - Large

Dropped old columns after feature creation.

### 4. Preprocessing

- One-Hot Encoding for categorical features
- StandardScaler for numeric features
- Train-test split (80-20)

### 5. Model Training

Trained and compared multiple models:

- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- SVM
- KNN
- Naive Bayes

---

## Model Performance

| Model | Accuracy |
|------|----------|
| Random Forest | 82.68% |
| KNN | 82.12% |
| Gradient Boosting | 81.56% |
| SVM | 81.56% |
| Logistic Regression | 80.45% |
| Decision Tree | 74.30% |
| Naive Bayes | 72.07% |

---

## Best Model

**Random Forest Classifier** achieved the highest accuracy:

**82.68%**

---

## Key Learnings

Through this project, I learned:

- Real-world data preprocessing
- Handling missing values
- EDA techniques
- Feature engineering
- Encoding categorical data
- Feature scaling
- Classification algorithms
- Model comparison
- Evaluation metrics
