# 🚢 Titanic Survival Prediction — Supervised Machine Learning Project

A **Supervised Machine Learning Classification** project using the **Titanic dataset** to predict passenger survival and compare multiple classification algorithms.

---

## 📌 Project Overview

This project focuses on analyzing the **Titanic dataset** and developing machine learning classification models to predict whether a passenger survived the Titanic disaster.

The project follows a complete **Supervised Machine Learning workflow**, including:

- **Data Understanding**
- **Exploratory Data Analysis (EDA)**
- **Data Cleaning**
- **Missing Value Handling**
- **Feature Selection**
- **Categorical Data Encoding**
- **Feature Scaling**
- **Train-Test Split**
- **Model Training**
- **Model Evaluation**
- **Model Comparison**

Multiple **classification algorithms** are implemented and compared to identify the **best-performing model**.

---

## 🎯 Objectives

The main objectives of this project are:

- Perform **Exploratory Data Analysis (EDA)** on the Titanic dataset.
- Understand the distribution and relationships between different features.
- Identify and handle **missing values**.
- Clean and preprocess the dataset for machine learning.
- Convert **categorical variables into numerical representations**.
- Perform **feature selection and preprocessing**.
- Apply **feature scaling** where required.
- Split the dataset into **training and testing data**.
- Train multiple **Supervised Machine Learning classification models**.
- Evaluate model performance using **classification metrics**.
- Compare different models and identify the **best-performing model**.

---

## 🎯 Problem Statement

The objective of this project is to predict whether a passenger **survived the Titanic disaster** based on passenger information.

### Target Variable

**`survived`**

- `0` → **Did Not Survive**
- `1` → **Survived**

---

## 📊 Dataset

The Titanic dataset contains information about **891 passengers**.

### Important Features

| Feature | Description |
|---|---|
| `survived` | **Survival status** |
| `pclass` | **Passenger class** |
| `sex` | **Gender** |
| `age` | **Age of passenger** |
| `sibsp` | **Number of siblings/spouses aboard** |
| `parch` | **Number of parents/children aboard** |
| `fare` | **Passenger fare** |
| `embarked` | **Port of embarkation** |

---

## 🔍 Exploratory Data Analysis

**Exploratory Data Analysis (EDA)** was performed to understand the dataset and identify important patterns.

The analysis includes:

- **Dataset structure**
- **Statistical information**
- **Missing values**
- **Survival distribution**
- **Passenger characteristics**
- **Feature relationships**
- **Data visualization**

Visualizations were created using **Matplotlib** and **Seaborn**.

---

## 🧹 Data Preprocessing

Before training the models, the dataset was cleaned and prepared.

The preprocessing steps include:

- **Handling missing values**
- **Removing unnecessary columns**
- **Encoding categorical features**
- **Separating features and target variable**
- **Splitting data into training and testing sets**
- **Applying feature scaling where required**

---

## ✂️ Train-Test Split

The dataset was divided into:

- **80% Training Data**
- **20% Testing Data**

The **training data** was used to train the machine learning models, while the **testing data** was used to evaluate their performance.

---

## ⚙️ Feature Scaling

Feature scaling was applied using **StandardScaler**.

Scaling is especially important for **distance-based** and **margin-based** algorithms such as:

- **K-Nearest Neighbors (KNN)**
- **Support Vector Machine (SVM)**

---

## 🤖 Machine Learning Models

The following **Supervised Machine Learning Classification algorithms** were implemented:

1. **Logistic Regression**
2. **K-Nearest Neighbors (KNN)**
3. **Naive Bayes**
4. **Decision Tree**
5. **Support Vector Machine (SVM)**

### 1️⃣ Logistic Regression

**Logistic Regression** is a supervised classification algorithm used to predict **binary outcomes**.

In this project, it predicts whether a passenger:

- **Survived**
- **Did not survive**

### 2️⃣ K-Nearest Neighbors (KNN)

**KNN** is a **distance-based machine learning algorithm**.

It classifies a new data point based on the classes of its **nearest neighboring data points**.

**Feature scaling** was applied before training the KNN model.

### 3️⃣ Naive Bayes

**Gaussian Naive Bayes** was used as a **probabilistic classification algorithm**.

It uses probability and **Bayes' theorem** to predict the class of a passenger.

### 4️⃣ Decision Tree

**Decision Tree** is a **tree-based supervised learning algorithm**.

It creates **decision rules** based on different passenger features and uses those rules to classify survival.

### 5️⃣ Support Vector Machine (SVM)

**Support Vector Machine (SVM)** finds the best **decision boundary** that separates different classes.

In this project, SVM was implemented using the **RBF (Radial Basis Function) Kernel**.

The **RBF Kernel** helps SVM handle **nonlinear relationships** in the dataset.

---

## 📈 Model Evaluation

The trained models were evaluated using multiple **classification metrics**.

The evaluation includes:

- **Accuracy Score**
- **Confusion Matrix**
- **Classification Report**
- **Precision**
- **Recall**
- **F1-Score**

---

## 🏆 Model Comparison

The performance of all **five classification models** was compared.

This helps determine which machine learning algorithm performs best on the **Titanic survival classification problem**.

According to the final model comparison in the notebook:

**Support Vector Machine (SVM) with RBF Kernel achieved the best performance among the tested models.**

---

## 🛠️ Technologies and Libraries

The project is implemented using **Python** and the following libraries:

- **Python**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Google Colab**
- **Jupyter Notebook**
- **GitHub**

---

## 📚 Machine Learning Concepts Covered

This project covers:

- **Supervised Learning**
- **Classification**
- **Exploratory Data Analysis**
- **Data Cleaning**
- **Missing Value Handling**
- **Feature Selection**
- **Label Encoding**
- **Feature Scaling**
- **Train-Test Split**
- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Naive Bayes**
- **Decision Tree**
- **Support Vector Machine (SVM)**
- **RBF Kernel**
- **Accuracy Score**
- **Confusion Matrix**
- **Precision**
- **Recall**
- **F1-Score**
- **Classification Report**
- **Model Comparison**

---

## 📁 Project Structure

```text
supervised-ml-classification-titanic/
│
├── titanic.ipynb
├── titanic_train.csv
├── titanic_model_ready.csv
├── titanic_best_model.joblib
├── Titanic_DataScience_Cleaning.pdf
├── README.md
└── requirements.txt
