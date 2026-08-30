🚢 Titanic Survival Prediction using Supervised Machine Learning

📌 Project Overview

This project uses the Titanic dataset to predict whether a passenger survived the Titanic disaster based on passenger-related features.

The project demonstrates the complete workflow of a Supervised Machine Learning Classification problem, including data exploration, data preprocessing, feature encoding, feature scaling, model training, prediction, and model evaluation.

Multiple classification algorithms are implemented and compared to identify the best-performing model.

⸻

🎯 Objective

The main objective of this project is to predict the survival status of Titanic passengers.

* Target Variable: survived
* 0 → Did not survive
* 1 → Survived

⸻

📊 Dataset

The Titanic dataset contains information about 891 passengers and initially includes 15 columns.

Important features include:

Feature	Description
survived	Survival status (Target)
pclass	Passenger class
sex	Passenger gender
age	Passenger age
sibsp	Number of siblings/spouses aboard
parch	Number of parents/children aboard
fare	Passenger fare
embarked	Port of embarkation

⸻

🔍 Data Preprocessing

The following preprocessing steps were performed:

1. Checked the dataset structure and statistics.
2. Checked for missing/null values.
3. Removed unnecessary columns:
    * deck
    * embark_town
    * alive
    * class
    * who
    * adult_male
4. Filled missing values in the age column using the mean.
5. Removed rows containing missing values in the embarked column.
6. Applied Label Encoding to categorical columns:
    * sex
    * embarked
7. Converted the dataset into integer format.
8. Split the data into training and testing sets using an 80:20 ratio.
9. Applied StandardScaler for feature scaling where required.

⸻

🤖 Machine Learning Algorithms

Five supervised classification algorithms were implemented:

1. Logistic Regression

A linear classification algorithm used as one of the baseline models.

2. K-Nearest Neighbors (KNN)

A distance-based classification algorithm. Feature scaling was applied because KNN depends on distances between data points.

3. Naive Bayes

The Gaussian Naive Bayes algorithm was used for classification.

4. Decision Tree

A tree-based supervised learning algorithm used to classify passengers based on their features.

5. Support Vector Machine (SVM)

SVM was implemented using the RBF (Radial Basis Function) kernel to handle nonlinear relationships in the data.

SVC(kernel='rbf', random_state=42)

⸻

📈 Model Evaluation

The models were evaluated using:

* Accuracy Score
* Confusion Matrix
* Classification Report

The classification report provides:

* Precision
* Recall
* F1-score
* Support

⸻

🏆 Model Comparison

After implementing multiple supervised learning algorithms, their performance was compared using accuracy scores.

According to the notebook’s final comparison, SVM achieved the best accuracy among the models tested.

Note: The exact accuracy values can be found in the Jupyter Notebook outputs.

⸻

🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab
* Jupyter Notebook

⸻

📚 Machine Learning Concepts Covered

This project covers the following concepts:

* Supervised Learning
* Classification
* Exploratory Data Analysis (EDA)
* Missing Value Handling
* Label Encoding
* Feature Scaling
* Train-Test Split
* Logistic Regression
* KNN
* Naive Bayes
* Decision Tree
* Support Vector Machine
* RBF Kernel
* Model Evaluation
* Confusion Matrix
* Classification Report
* Model Comparison

⸻

📁 Project Structure

supervised-ml-classification-titanic/
│
├── titanic.ipynb
├── README.md
└── requirements.txt

⸻

▶️ How to Run

Using Google Colab

1. Open the notebook in Google Colab.
2. Run the cells sequentially.
3. The Titanic dataset is loaded using Seaborn.
4. Follow the preprocessing and model-training steps.
5. Compare the performance of the different models.

Using Jupyter Notebook

Install the required libraries:

pip install numpy pandas matplotlib seaborn scikit-learn

Then open:

titanic.ipynb

⸻

💡 Key Learning

This project demonstrates how different supervised machine learning algorithms can be applied to the same classification problem and evaluated using common performance metrics.

It also demonstrates why feature preprocessing and scaling are important for algorithms such as KNN and SVM.

⸻

👨‍💻 Author

Aditya Raj

B.Tech – Data Science

⸻

⭐ Conclusion

The Titanic Survival Prediction project provides practical experience with the complete supervised machine learning pipeline, from data preprocessing to model evaluation and comparison.

Among the implemented models, Support Vector Machine with an RBF kernel achieved the best accuracy according to the notebook’s final comparison.
