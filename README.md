# Comparison of Classification Algorithms for Heart Disease Prediction

A machine learning project that compares multiple classification algorithms for heart disease prediction using data preprocessing, exploratory data analysis (EDA), feature selection, and performance evaluation.

---

## Project Overview

Heart disease is one of the leading causes of death worldwide. Early prediction using machine learning can assist healthcare professionals in making faster and more accurate clinical decisions.

This project presents a comparative analysis of four supervised machine learning algorithms to predict heart disease using the publicly available Heart Disease Dataset. The project follows a complete machine learning pipeline, including data preprocessing, exploratory data analysis (EDA), feature selection, model training, and performance evaluation.

The primary objective is to identify the most effective classification algorithm based on several evaluation metrics.

---

## Algorithms

The following machine learning algorithms are implemented and compared:

- Naive Bayes
- Decision Tree
- K-Nearest Neighbor (KNN)
- Logistic Regression

---

## Dataset

**Dataset:** Heart Disease Dataset

- Total Records : **1,190**
- Total Features : **11**
- Target Classes : **2 (Heart Disease / Normal)**

The dataset contains clinical information such as:

- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol
- Fasting Blood Sugar
- Resting ECG
- Maximum Heart Rate
- Exercise-Induced Angina
- Oldpeak
- ST Slope

---

## Machine Learning Workflow

```
Dataset
    │
    ▼
Data Preprocessing
    │
    ▼
Exploratory Data Analysis (EDA)
    │
    ▼
Feature Selection (Chi-Square)
    │
    ▼
Model Training
    │
    ▼
Model Evaluation
    │
    ▼
Best Model Selection
```

---



## Feature Selection

Feature selection was performed using:

- **SelectKBest**
- **Chi-Square Test**

This approach helps identify the most informative features while reducing model complexity.

---

## Model Evaluation

Each classification model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### Performance Summary

| Algorithm | Accuracy |
|-----------|---------:|
| Decision Tree | **89.92%** |
| K-Nearest Neighbor | 88.66% |
| Logistic Regression | 86.13% |
| Naive Bayes | 85.71% |

Based on the experimental results, the **Decision Tree** classifier achieved the highest overall performance and was selected as the best-performing model for heart disease prediction.

---

## Repository Structure

```
comparison-of-classification-algorithms-for-heart-disease-prediction/
│
├── data/
│   └── heart_statlog_cleveland_hungary_final.csv
│
├── model/
│   ├── heart_disease_model.pkl
│   └── scaler.pkl
│
├── notebooks/
│   └── Comparison-of-Classification-Algorithms-for-Heart-Disease-Prediction.ipynb
│
└── README.md
```


---

## Requirements

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib notebook
```

---

## How to Run

1. Clone this repository.

```bash
git clone https://github.com/ddaannuu/comparison-of-classification-algorithms-for-heart-disease-prediction.git
```

2. Navigate to the project directory.

```bash
cd comparison-of-classification-algorithms-for-heart-disease-prediction
```

3. Open the notebook.

```
notebooks/
└── Comparison-of-Classification-Algorithms-for-Heart-Disease-Prediction.ipynb
```

4. Run all notebook cells sequentially.
