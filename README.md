# Predicting Stellar Class

A Machine Learning project that classifies celestial objects into **Galaxy**, **Quasar (QSO)**, and **Star** using astronomical observation data. This project was developed as a solution for the Kaggle Playground Series S6E6 competition.

## Problem Statement

Astronomical surveys collect massive amounts of observational data. The goal of this project is to build a machine learning model capable of accurately classifying celestial objects into one of the following classes:

* GALAXY
* QSO (Quasi-Stellar Object / Quasar)
* STAR

## Dataset

The dataset consists of numerical and categorical astronomical features describing observed celestial objects.

* Training Samples: 577,347+
* Target Variable: `class`
* Classes:

  * GALAXY
  * QSO
  * STAR

## Project Workflow

### 1. Data Loading

* Loaded training and test datasets using Pandas.

### 2. Data Preprocessing

#### Numerical Features

* Standardized using `StandardScaler`.

#### Categorical Features

* Encoded using `OneHotEncoder`.

### 3. Target Encoding

| Class  | Encoded Value |
| ------ | ------------- |
| GALAXY | 0             |
| QSO    | 1             |
| STAR   | 2             |

### 4. Feature Engineering

* Combined scaled numerical features and one-hot encoded categorical features into a single feature matrix.

### 5. Model Training

The following machine learning models were trained and evaluated:

* Logistic Regression
* Random Forest Classifier
* Gradient Boosting Classifier

### 6. Model Comparison

Training accuracy was compared across all three models using a bar chart visualization.

### 7. Prediction & Submission

The Random Forest model was used to generate predictions for the test dataset.

Predicted labels were converted back to their original class names:

* 0 → GALAXY
* 1 → QSO
* 2 → STAR

Final predictions were exported as:

```text
Stellar_Class_Submission.csv
```

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* Matplotlib

## Libraries

```python
pandas
numpy
scikit-learn
matplotlib
```

## Project Structure

```text
Predicting-Stellar-Class/
│
├── Predicting_Stellar_Class.ipynb
├── Stellar_Class_Submission.csv
├── README.md
└── dataset/
```

## Key Learning Outcomes

* Data preprocessing for mixed-type datasets
* One-Hot Encoding
* Feature Scaling
* Multi-class Classification
* Model Comparison
* Kaggle Competition Workflow
* Submission File Generation

## Future Improvements

* Hyperparameter Tuning
* Cross Validation
* XGBoost
* LightGBM
* CatBoost
* Feature Importance Analysis
* Ensemble Methods

## Author

Abhiram

Aspiring AI/ML Engineer
