# 🚢 Titanic Survival Prediction — Supervised Machine Learning Project

A Supervised Machine Learning Classification project using the Titanic dataset to predict passenger survival and compare multiple classification algorithms.

---

## 📌 Project Overview

This project focuses on analyzing the Titanic dataset and developing machine learning classification models to predict whether a passenger survived the Titanic disaster.

The project follows a complete Supervised Machine Learning workflow, including:

- Data Understanding
- Exploratory Data Analysis (EDA)
- Data Cleaning
- Missing Value Handling
- Feature Selection
- Categorical Data Encoding
- Feature Scaling
- Train-Test Split
- Model Training
- Model Evaluation
- Model Comparison

Multiple classification algorithms are implemented and compared to identify the best-performing model.

---

## 🎯 Objectives

The main objectives of this project are:

- Perform Exploratory Data Analysis (EDA) on the Titanic dataset.
- Understand the distribution and relationships between different features.
- Identify and handle missing values.
- Clean and preprocess the dataset for machine learning.
- Convert categorical variables into numerical representations.
- Perform feature selection and preprocessing.
- Apply feature scaling where required.
- Split the dataset into training and testing data.
- Train multiple Supervised Machine Learning classification models.
- Evaluate model performance using classification metrics.
- Compare different models and identify the best-performing model.

---

## 🎯 Problem Statement

The objective of this project is to predict whether a passenger survived the Titanic disaster based on passenger information.

### Target Variable

survived

- 0 → Did Not Survive
- 1 → Survived

---

## 📊 Dataset

The Titanic dataset contains information about 891 passengers.

### Important Features

| Feature | Description |
|---|---|
| survived | Survival status |
| pclass | Passenger class |
| sex | Gender |
| age | Age of passenger |
| sibsp | Number of siblings/spouses aboard |
| parch | Number of parents/children aboard |
| fare | Passenger fare |
| embarked | Port of embarkation |

---

## 🔍 Exploratory Data Analysis

Exploratory Data Analysis (EDA) was performed to understand the dataset and identify important patterns.

The analysis includes:

- Dataset structure
- Statistical information
- Missing values
- Survival distribution
- Passenger characteristics
- Feature relationships
- Data visualization

Visualizations were created using Matplotlib and Seaborn.

---

## 🧹 Data Preprocessing

Before training the models, the dataset was cleaned and prepared.

The preprocessing steps include:

- Handling missing values
- Removing unnecessary columns
- Encoding categorical features
- Separating features and target variable
- Splitting data into training and testing sets
- Applying feature scaling where required

### Missing Value Handling

Missing values in the age column were handled using the mean value.

Missing records in the embarked column were removed before model training.

### Removing Unnecessary Features

The following unnecessary or redundant columns were removed:

- deck
- embark_town
- alive
- class
- who
- adult_male

---

## 🔢 Categorical Data Encoding

Categorical variables were converted into numerical representations using Label Encoding.

The following categorical features were encoded:

- sex
- embarked

This conversion allows machine learning algorithms to process categorical information as numerical input.

---

## 🎯 Feature and Target Separation

The dataset was divided into input features and the target variable.

X = df.drop(['survived'], axis=1)
y = df['survived']

Where:

- X → Input features
- y → Target variable (survived)

---

## ✂️ Train-Test Split

The dataset was divided into:

- 80% Training Data
- 20% Testing Data

The training data was used to train the machine learning models, while the testing data was used to evaluate their performance on unseen data.

The dataset was split using:

X_train, X_test, y_train, y_test = train_test_split(
    X,
    y,
    test_size=0.2,
    random_state=42
)

---

## ⚙️ Feature Scaling

Feature scaling was applied using StandardScaler.

Scaling is especially important for algorithms that are sensitive to feature magnitude, such as:

- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)

Standardization brings numerical features to a comparable scale.

---

## 🤖 Machine Learning Models

The following Supervised Machine Learning Classification algorithms were implemented:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Naive Bayes
4. Decision Tree
5. Support Vector Machine (SVM)

---

## 1️⃣ Logistic Regression

Logistic Regression is a supervised classification algorithm used to predict binary outcomes.

In this project, it is used to predict whether a Titanic passenger:

- Survived
- Did not survive

### Result

Accuracy: 80.34%

### Confusion Matrix

[[90 19]
 [16 53]]

---

## 2️⃣ K-Nearest Neighbors (KNN)

K-Nearest Neighbors (KNN) is a distance-based classification algorithm.

It classifies a new data point based on the classes of its nearest neighboring data points.

Feature scaling was applied before training the KNN model because KNN relies on distance calculations.

### Result

Accuracy: 77.53%

### Confusion Matrix

[[89 20]
 [20 49]]

---

## 3️⃣ Naive Bayes

Gaussian Naive Bayes is a probabilistic classification algorithm based on Bayes' theorem.

It calculates the probability of different classes and predicts the most likely class.

### Result

Accuracy: 77.53%

### Confusion Matrix

[[84 25]
 [15 54]]

---

## 4️⃣ Decision Tree

Decision Tree is a tree-based supervised learning algorithm.

It creates a series of decision rules based on different passenger features and uses those rules to classify passenger survival.

### Result

Accuracy: 76.97%

### Confusion Matrix

[[88 21]
 [20 49]]

---

## 5️⃣ Support Vector Machine (SVM)

Support Vector Machine (SVM) finds the best decision boundary that separates different classes.

In this project, SVM was implemented using the RBF (Radial Basis Function) Kernel.

The RBF Kernel helps SVM handle nonlinear relationships in the dataset.

SVM implementation:

from sklearn.svm import SVC

model_svm = SVC(
    kernel='rbf',
    random_state=42
)

### Result

Accuracy: 82.58%

### Confusion Matrix

[[96 13]
 [18 51]]

---

## 📈 Model Evaluation

The trained models were evaluated using multiple classification metrics.

The evaluation includes:

- Accuracy Score
- Confusion Matrix
- Classification Report
- Precision
- Recall
- F1-Score

### Accuracy Score

Accuracy measures the percentage of predictions that were correctly classified.

Accuracy = Correct Predictions / Total Predictions

### Classification Report

The Classification Report provides:

- Precision
- Recall
- F1-Score
- Support

### Confusion Matrix

The Confusion Matrix helps understand correct and incorrect predictions.

It contains:

- True Positive
- True Negative
- False Positive
- False Negative

---

## 🏆 Model Comparison

The performance of all five classification models was compared using their Accuracy Scores.

| Model | Accuracy |
|---|---:|
| Logistic Regression | 80.34% |
| K-Nearest Neighbors (KNN) | 77.53% |
| Naive Bayes | 77.53% |
| Decision Tree | 76.97% |
| Support Vector Machine (SVM) | 82.58% |

### 🥇 Best Performing Model

Among the tested models:

Support Vector Machine (SVM) with RBF Kernel achieved the highest accuracy of 82.58%.

Therefore, based on the model comparison, SVM is the best-performing model among the implemented classification algorithms.

---

## 🛠️ Technologies and Libraries

The project is implemented using Python and the following libraries:

- Python — Programming Language
- NumPy — Numerical Computing
- Pandas — Data Manipulation and Analysis
- Matplotlib — Data Visualization
- Seaborn — Data Visualization and Analysis
- Scikit-learn — Machine Learning and Preprocessing
- Google Colab — Notebook Environment
- Jupyter Notebook — Interactive Development Environment
- GitHub — Project Hosting and Version Control

---

## 📚 Machine Learning Concepts Covered

This project covers:

- Supervised Learning
- Binary Classification
- Exploratory Data Analysis
- Data Cleaning
- Missing Value Handling
- Feature Selection
- Categorical Encoding
- Label Encoding
- Feature Scaling
- StandardScaler
- Train-Test Split
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Naive Bayes
- Decision Tree
- Support Vector Machine (SVM)
- RBF Kernel
- Accuracy Score
- Confusion Matrix
- Precision
- Recall
- F1-Score
- Classification Report
- Model Comparison

---

## 📁 Project Structure

supervised-ml-classification-titanic/
│
├── titanic.ipynb
├── titanic_train.csv
├── titanic_model_ready.csv
├── titanic_best_model.joblib
├── Titanic_DataScience_Cleaning.pdf
└── README.md

---

## 🚀 How to Run the Project

### 1. Clone the Repository

git clone https://github.com/Adityashahi2125/supervised-ml-classification-titanic.git

### 2. Navigate to the Project

cd supervised-ml-classification-titanic

### 3. Install Required Libraries

pip install numpy pandas matplotlib seaborn scikit-learn

### 4. Open the Notebook

Open:

titanic.ipynb

The notebook can be opened using:

- Google Colab
- Jupyter Notebook

### 5. Run the Notebook

Run all notebook cells sequentially to perform:

Data Understanding → Data Cleaning → Encoding → Feature Scaling → Train-Test Split → Model Training → Prediction → Evaluation → Model Comparison

---

## 📌 Key Machine Learning Workflow

Raw Titanic Dataset
        ↓
Data Understanding
        ↓
Exploratory Data Analysis
        ↓
Missing Value Checking
        ↓
Data Cleaning
        ↓
Remove Unnecessary Features
        ↓
Missing Value Handling
        ↓
Categorical Encoding
        ↓
Feature & Target Separation
        ↓
Train-Test Split
        ↓
Feature Scaling
        ↓
Model Training
        ↓
Prediction
        ↓
Model Evaluation
        ↓
Model Comparison
        ↓
Best Model Selection

---

## 💡 Key Learning

This project provides practical experience with the complete Supervised Machine Learning Classification pipeline.

It demonstrates how raw Titanic passenger data is:

Analyzed → Cleaned → Preprocessed → Encoded → Scaled → Split → Used for Model Training → Evaluated → Compared

The project also provides practical understanding of how different classification algorithms perform on the same dataset.

The model comparison shows that Support Vector Machine (SVM) with RBF Kernel achieved the highest accuracy among the implemented models.

---

## 🚀 Future Improvements

The project can be improved further by:

- Hyperparameter Tuning
- Cross-Validation
- Advanced Feature Engineering
- Random Forest Implementation
- Gradient Boosting Models
- ROC-AUC Comparison
- Detailed Error Analysis
- Improved Feature Selection
- SVM Parameter Optimization
- Model Deployment using Streamlit
- Creating a web-based Titanic Survival Prediction Application

---

## 👨‍💻 Author

Aditya Raj

B.Tech – Data Science

---

## ⭐ Project Highlights

Data Understanding → Exploratory Data Analysis → Data Cleaning → Missing Value Handling → Feature Selection → Categorical Encoding → Feature Scaling → Train-Test Split → Supervised Learning → Classification → Model Training → Model Evaluation → Model Comparison → Best Model Selection

### 🏆 Best Model

Support Vector Machine (SVM) with RBF Kernel

Accuracy: 82.58%
