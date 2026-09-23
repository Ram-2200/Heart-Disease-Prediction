# Heart Disease Prediction using Machine Learning

A machine learning project that predicts the presence of heart disease using clinical features and classification algorithms in Python.

## Project Overview

This project explores the use of machine learning for binary classification of heart disease using the UCI Heart Disease dataset.

The notebook covers:

- Data loading and preprocessing
- Exploratory data analysis
- Feature analysis and correlation
- Train-test split
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Random Forest Classifier
- Model evaluation
- Heart disease prediction

## Dataset

The project uses a heart disease dataset containing 303 patient records and 13 input features.

The target variable represents the classification:

- `1` — Heart disease present
- `0` — Heart disease absent

### Features

| Feature | Description |
|---|---|
| age | Age of the patient |
| sex | Sex |
| cp | Chest pain type |
| trestbps | Resting blood pressure |
| chol | Serum cholesterol |
| fbs | Fasting blood sugar |
| restecg | Resting ECG results |
| thalach | Maximum heart rate achieved |
| exang | Exercise-induced angina |
| oldpeak | ST depression |
| slope | Slope of peak exercise ST segment |
| ca | Number of major vessels |
| thal | Thalassemia |
| target | Prediction target |

## Machine Learning Algorithms

The project experiments with:

1. Logistic Regression
2. K-Nearest Neighbors
3. Random Forest Classifier

### Results

The notebook currently reports:

| Model | Evaluation |
|---|---:|
| Logistic Regression | 81.97% test accuracy |
| KNN | 84.48% mean 10-fold cross-validation score |
| Random Forest | 79.49% mean 10-fold cross-validation score |

These results are based on the current notebook implementation and dataset.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

## Project Structure

```text
Heart-Disease-Prediction/
│
├── data.csv
├── heart_disease_prediction.ipynb
└── README.md
