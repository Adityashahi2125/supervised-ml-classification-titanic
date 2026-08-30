🚢 Titanic Survival Prediction

A Supervised Machine Learning Classification project using the Titanic dataset to predict passenger survival and compare multiple classification algorithms.

📌 Project Overview

This project demonstrates a complete Supervised Machine Learning workflow using the Titanic dataset.

The project includes:

* Data Understanding
* Exploratory Data Analysis (EDA)
* Data Cleaning
* Missing Value Handling
* Feature Selection
* Categorical Data Encoding
* Feature Scaling
* Train-Test Split
* Model Training
* Model Evaluation
* Model Comparison

Multiple classification algorithms are implemented and compared to identify the best-performing model.

🎯 Problem Statement

The objective of this project is to predict whether a passenger survived the Titanic disaster based on passenger information.

Target Variable

survived

* 0 → Did Not Survive
* 1 → Survived

📊 Dataset

The Titanic dataset contains information about 891 passengers.

Important Features

Feature	Description
survived	Survival status
pclass	Passenger class
sex	Gender
age	Age of passenger
sibsp	Number of siblings/spouses aboard
parch	Number of parents/children aboard
fare	Passenger fare
embarked	Port of embarkation

🔍 Exploratory Data Analysis

Exploratory Data Analysis (EDA) was performed to understand the dataset and identify important patterns.

The analysis includes:

* Dataset structure
* Statistical information
* Missing values
* Survival distribution
* Passenger characteristics
* Feature relationships
* Data visualization

Visualizations were created using Matplotlib and Seaborn.

🧹 Data Preprocessing

Before training the models, the dataset was cleaned and prepared.

The preprocessing steps include:

* Handling missing values
* Removing unnecessary columns
* Encoding categorical features
* Separating features and target variable
* Splitting data into training and testing sets
* Applying feature scaling where required

✂️ Train-Test Split

The dataset was divided into:

* 80% Training Data
* 20% Testing Data

The training data was used to train the machine learning models, while the testing data was used to evaluate their performance.

⚙️ Feature Scaling

Feature scaling was applied using StandardScaler.

Scaling is especially important for distance-based and margin-based algorithms such as:

* K-Nearest Neighbors (KNN)
* Support Vector Machine (SVM)

🤖 Machine Learning Models

The following Supervised Machine Learning Classification algorithms were implemented:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Naive Bayes
4. Decision Tree
5. Support Vector Machine (SVM)

1️⃣ Logistic Regression

Logistic Regression is a supervised classification algorithm used to predict binary outcomes.

In this project, it predicts whether a passenger:

* Survived
* Did not survive

2️⃣ K-Nearest Neighbors (KNN)

KNN is a distance-based machine learning algorithm.

It classifies a new data point based on the classes of its nearest neighboring data points.

Feature scaling was applied before training the KNN model.

3️⃣ Naive Bayes

Gaussian Naive Bayes was used as a probabilistic classification algorithm.

It uses probability and Bayes’ theorem to predict the class of a passenger.

4️⃣ Decision Tree

Decision Tree is a tree-based supervised learning algorithm.

It creates decision rules based on different passenger features and uses those rules to classify survival.

5️⃣ Support Vector Machine (SVM)

Support Vector Machine (SVM) finds the best decision boundary that separates different classes.

In this project, SVM was implemented using the RBF (Radial Basis Function) Kernel.

The RBF Kernel helps SVM handle nonlinear relationships in the dataset.

📈 Model Evaluation

The trained models were evaluated using multiple classification metrics.

The evaluation includes:

* Accuracy Score
* Confusion Matrix
* Classification Report
* Precision
* Recall
* F1-Score

🏆 Model Comparison

The performance of all five classification models was compared.

This helps determine which machine learning algorithm performs best on the Titanic survival classification problem.

According to the final model comparison in the notebook, Support Vector Machine (SVM) with RBF Kernel achieved the best performance among the tested models.

🛠️ Technologies Used

Programming Language

* Python

Libraries

* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn

Tools

* Google Colab
* Jupyter Notebook
* GitHub

📚 Machine Learning Concepts Covered

This project covers:

* Supervised Learning
* Classification
* Exploratory Data Analysis (EDA)
* Data Cleaning
* Missing Value Handling
* Feature Selection
* Label Encoding
* Feature Scaling
* Train-Test Split
* Logistic Regression
* K-Nearest Neighbors (KNN)
* Naive Bayes
* Decision Tree
* Support Vector Machine (SVM)
* RBF Kernel
* Accuracy Score
* Confusion Matrix
* Precision
* Recall
* F1-Score
* Classification Report
* Model Comparison

📁 Project Structure

titanic-survival-prediction/
│
├── titanic.ipynb
├── README.md
└── requirements.txt

▶️ How to Run

1. Clone or download this repository.
2. Open titanic.ipynb using Google Colab or Jupyter Notebook.
3. Install the required Python libraries.
4. Run all notebook cells sequentially.
5. Check the model evaluation and comparison results.

📦 Required Libraries

pip install numpy pandas matplotlib seaborn scikit-learn

💡 Key Learning

This project provides practical experience with the complete Supervised Machine Learning Classification pipeline.

It demonstrates how raw data is cleaned and transformed before training multiple machine learning models and comparing their performance.

🚀 Future Improvements

The project can be improved further by:

* Hyperparameter Tuning
* Cross-Validation
* Feature Engineering
* Random Forest Implementation
* Gradient Boosting Models
* ROC-AUC Comparison
* Model Deployment using Streamlit

👨‍💻 Author

Aditya Raj

B.Tech – Data Science

⭐ Conclusion

This project demonstrates an end-to-end Supervised Machine Learning Classification workflow using the Titanic dataset.

Multiple classification algorithms were trained and evaluated, including:

Logistic Regression, KNN, Naive Bayes, Decision Tree, and Support Vector Machine.

The project provides practical understanding of data preprocessing, model training, evaluation, and comparison of supervised machine learning algorithms.
