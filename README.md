
# ❤️ Heart Disease Prediction using Machine Learning

<p align="center">
  <strong>Machine Learning Classification Project using Python & Scikit-learn</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas" alt="Pandas">
  <img src="https://img.shields.io/badge/Scikit--learn-Machine%20Learning-F7931E?logo=scikit-learn" alt="Scikit-learn">
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter" alt="Jupyter">
</p>

---

## 📌 Project Overview

This project explores machine learning techniques for predicting the presence of heart disease using clinical features.

The project uses Python and Scikit-learn to perform data analysis, preprocessing, model training, evaluation, and prediction.

The notebook experiments with multiple classification algorithms and compares their performance.

> **Note:** This project is created for educational and machine learning practice purposes. It is not a medical diagnostic system.

---

## 🔄 Machine Learning Workflow

```text
Dataset
   ↓
Data Collection
   ↓
Data Exploration
   ↓
Data Cleaning
   ↓
Feature / Target Separation
   ↓
Train-Test Split
   ↓
Feature Scaling & Processing
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Model Comparison
   ↓
Prediction
````

---

## 📊 Dataset

The dataset contains:

* **303 records**
* **13 input features**
* **1 target variable**

### Target Variable

| Value | Meaning               |
| ----- | --------------------- |
| `1`   | Heart disease present |
| `0`   | Heart disease absent  |

### Features

| Feature    | Meaning                           |
| ---------- | --------------------------------- |
| `age`      | Age of the patient                |
| `sex`      | Sex                               |
| `cp`       | Chest pain type                   |
| `trestbps` | Resting blood pressure            |
| `chol`     | Serum cholesterol                 |
| `fbs`      | Fasting blood sugar               |
| `restecg`  | Resting ECG results               |
| `thalach`  | Maximum heart rate achieved       |
| `exang`    | Exercise-induced angina           |
| `oldpeak`  | ST depression                     |
| `slope`    | Slope of peak exercise ST segment |
| `ca`       | Number of major vessels           |
| `thal`     | Thalassemia                       |

---

# 🤖 Machine Learning Models

The project experiments with the following classification algorithms:

### 1. Logistic Regression

A supervised classification algorithm that estimates the probability of a binary outcome.

**Revision:**

* Used for classification
* Produces probability-based predictions
* Uses a logistic/sigmoid function
* Common baseline model for binary classification

---

### 2. K-Nearest Neighbors (KNN)

KNN predicts the class of a new observation based on the classes of its nearest data points.

**Revision:**

* `K` = number of neighbors considered
* Distance-based algorithm
* Feature scaling is important
* Small `K` can be sensitive to noise
* Large `K` can make the model less sensitive to local patterns

---

### 3. Random Forest

Random Forest combines multiple decision trees to make predictions.

**Revision:**

* Ensemble learning algorithm
* Uses multiple decision trees
* Can reduce overfitting compared with a single decision tree
* Can capture nonlinear relationships
* `n_estimators` controls the number of trees

---

# 📈 Model Results

The current notebook reports:

| Model               |                                     Result |
| ------------------- | -----------------------------------------: |
| Logistic Regression |                       81.97% Test Accuracy |
| KNN                 | 84.48% Mean 10-Fold Cross-Validation Score |
| Random Forest       | 79.49% Mean 10-Fold Cross-Validation Score |

> These results represent the current notebook implementation and should not be interpreted as medical performance.

---

# 🧠 Machine Learning Revision Notes

Short notes for revising the concepts used in this project.

## Supervised Learning

Learning from labelled data where the input features and expected output are known.

Example:

```text
Patient Features → Model → Heart Disease Class
```

---

## Classification

A machine learning task where the output belongs to a category or class.

Example:

```text
0 → Heart disease absent
1 → Heart disease present
```

---

## Features

Input variables used by the model to make a prediction.

Examples:

```text
age
chol
trestbps
thalach
```

---

## Target

The variable that the model tries to predict.

In this project:

```text
target
```

---

## Train-Test Split

The dataset is divided into:

* **Training data** → used to learn the model
* **Testing data** → used to evaluate the model on unseen data

```text
Dataset
 ├── Training Set
 └── Test Set
```

---

## Feature Scaling

Feature scaling puts numerical features on comparable scales.

A common method is Standardization:

```text
z = (x - mean) / standard deviation
```

Scaling is especially important for distance-based algorithms such as KNN.

---

## Cross-Validation

Cross-validation evaluates a model across multiple train/test splits.

In 10-fold cross-validation:

```text
Dataset
   ↓
10 parts
   ↓
Train on 9 parts
Test on 1 part
   ↓
Repeat 10 times
   ↓
Average the scores
```

---

## Accuracy

Accuracy measures the percentage of predictions that are correct.

```text
Accuracy =
Correct Predictions / Total Predictions
```

---

## Confusion Matrix

A confusion matrix summarizes classification predictions.

|                 | Predicted Positive | Predicted Negative |
| --------------- | -----------------: | -----------------: |
| Actual Positive |      True Positive |     False Negative |
| Actual Negative |     False Positive |      True Negative |

---

## Overfitting

Overfitting occurs when a model learns the training data too closely and performs poorly on unseen data.

```text
High Training Performance
          ↓
Poor Test Performance
          ↓
Possible Overfitting
```

---

## Underfitting

Underfitting occurs when a model is too simple to capture important patterns in the data.

---

## Random State

`random_state` is used to make randomized operations reproducible.

Example:

```python
train_test_split(
    X,
    y,
    test_size=0.2,
    random_state=42
)
```

Using the same random state produces the same split.

---

# 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook
* Google Colab

---

# 📁 Project Structure

```text
Heart-Disease-Prediction/
│
├── data.csv
├── heart_disease_prediction.ipynb
└── README.md
```

---

# ▶️ How to Run

## Using Google Colab

1. Open the notebook.
2. Upload `data.csv` to the Colab environment.
3. Open `heart_disease_prediction.ipynb`.
4. Run the notebook cells sequentially.

## Using Jupyter Notebook

Install the required libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

Then start Jupyter:

```bash
jupyter notebook
```

Make sure `data.csv` is available in the notebook's working directory.

---

# ⚠️ Disclaimer

This project is intended for educational and machine learning practice purposes only.

It is **not a medical diagnostic system** and should not be used to make real-world medical decisions.

---

# 👨‍💻 Author

**Prateek Satpathi**

GitHub: [@Ram-2200](https://github.com/Ram-2200)

---

## 📚 Learning Focus

This project helped me practice:

* Python
* Pandas
* NumPy
* Exploratory Data Analysis
* Data preprocessing
* Classification
* Logistic Regression
* KNN
* Random Forest
* Model evaluation
* Cross-validation
* Machine learning fundamentals

```
