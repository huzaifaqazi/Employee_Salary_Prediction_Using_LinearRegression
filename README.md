# Employee Salary Prediction Using Machine Learning

## Project Overview

This project demonstrates a complete Machine Learning workflow for predicting employee salaries based on different features such as age, gender, and city. The project covers data preprocessing, feature engineering, model training, evaluation, and prediction.

---

## Dataset Description

The dataset contains employee information including:

- Age
- Gender
- City
- Salary (Target Variable)

The goal is to train a machine learning model that can predict an employee's salary using the available features.

---

## Project Workflow

### 1. Importing Required Libraries

Necessary Python libraries were imported for:

- Data manipulation (Pandas, NumPy)
- Data visualization (Matplotlib, Seaborn)
- Data preprocessing (Scikit-Learn)
- Machine Learning modeling
- Model evaluation

---

### 2. Loading the Dataset

The dataset was loaded into a Pandas DataFrame and explored to understand its structure, data types, and missing values.

---

### 3. Handling Missing Values

Missing values were identified and handled using appropriate imputation techniques to ensure data quality before training the model.

Purpose:
- Improve dataset consistency
- Prevent model training errors
- Increase prediction accuracy

---

### 4. Encoding Categorical Variables

Machine Learning models cannot directly process text values.

Categorical columns such as:

- Gender
- City

were converted into numerical format using:

- Label Encoding
- One-Hot Encoding

Purpose:
- Transform categorical data into machine-readable format.

---

### 5. Feature Scaling and Normalization

Feature scaling techniques were applied to bring all variables to a similar range.

Techniques used:

- StandardScaler
- MinMaxScaler

Purpose:
- Improve model performance
- Speed up convergence
- Reduce bias caused by different feature scales

---

### 6. Feature and Target Selection

The dataset was divided into:

#### Features (X)

- Age
- Gender
- City variables

#### Target (Y)

- Salary

The target variable represents the value that the model learns to predict.

---

### 7. Splitting the Dataset

The dataset was divided into:

- Training Set (80%)
- Testing Set (20%)

Purpose:
- Train the model on one portion of data
- Evaluate performance on unseen data

---

### 8. Model Training

A Linear Regression model was trained using the training dataset.

Linear Regression learns the relationship between employee attributes and salary values.

Purpose:
- Build a predictive model for salary estimation

---

### 9. Model Evaluation

The trained model was evaluated using metrics such as:

- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

These metrics measure how accurately the model predicts salaries.

---

### 10. Salary Prediction

After training, the model was used to predict salaries for new employee records.

Example Output:

```python
Prediction: [0.25697626 1.22300862]
```

These values represent the model's predicted salary values. Since MinMaxScaler was applied to the target variable, predictions are returned in normalized form and can be converted back to actual salary values using inverse transformation.

---

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook
---
## Machine Learning Algorithm

### Linear Regression

Linear Regression is a supervised machine learning algorithm used to predict continuous numerical values. In this project, it is used to estimate employee salaries based on available employee information.

---
 encoding, scaling, model training, evaluation, and prediction. The trained Linear Regression model can estimate salaries for new employee data and serves as a practical example of applying machine learning techniques to real-world business problems.
