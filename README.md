# Medical Insurance Cost Prediction and High-Risk Patient Classification

## Project Overview

This machine learning project analyzes medical insurance data to:

1. Predict individual medical insurance charges using regression.
2. Identify high-risk patients based on their medical insurance costs.
3. Analyze the factors that contribute to higher medical expenses.

The project was developed as part of the MS Artificial Intelligence program.

## Author

**Mehar Ali**

MS Artificial Intelligence

---

## Objectives

### 1. Medical Cost Prediction

Predict medical insurance charges using demographic and health-related features such as:

- Age
- Sex
- BMI
- Number of children/dependents
- Smoking status
- Region

A Linear Regression model is used for the prediction task.

### 2. High-Risk Patient Classification

Patients whose insurance charges are above the 75th percentile are classified as **high-risk**.

A Decision Tree Classifier is used to predict whether a patient belongs to the high-risk category.

### 3. Feature Analysis

The project analyzes important factors associated with medical costs, including:

- Age
- BMI
- Smoking status
- Number of children
- Region

---

## Dataset

The dataset contains the following variables:

| Feature | Description |
|---|---|
| `age` | Age of the individual |
| `sex` | Gender |
| `bmi` | Body Mass Index |
| `children` | Number of children/dependents |
| `smoker` | Smoking status |
| `region` | Geographical region |
| `charges` | Medical insurance charges |

The dataset contains **1,338 records**.

---

## Data Preprocessing

The following preprocessing steps were performed:

- Checked for missing values
- Encoded categorical variables
- Created BMI categories
- Created age groups
- Applied one-hot encoding to engineered categorical features
- Created a binary `high_risk` target variable

The high-risk threshold is defined using the 75th percentile of medical insurance charges.

Patients above this threshold are assigned:

- `1` → High Risk
- `0` → Normal Risk

The resulting dataset contains 1,003 normal-risk records and 335 high-risk records.

---

## Exploratory Data Analysis

The project includes visual analysis of relationships between medical charges and:

- Age
- BMI
- Smoking status
- Number of children

Visualizations include scatter plots and box plots.

---

## Machine Learning Models

### Regression

**Model:**
- Linear Regression

**Evaluation Metrics:**
- RMSE
- R² Score

The regression model is used to predict individual medical insurance charges.

### Classification

**Model:**
- Decision Tree Classifier

**Evaluation Metrics:**
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

The decision tree is also visualized to interpret the classification process.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- Jupyter Notebook

---

## Project Structure

```text
Machine-Learning-Projects/
│
├── Medical_Insurance_Cost_Prediction_and_High_Risk_Patient_Classification_By_Mehar_Ali.ipynb
└── README.md
