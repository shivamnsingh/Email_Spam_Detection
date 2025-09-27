📧 Email Spam Detection

🔍 Project Overview

This project classifies emails as spam or ham using three popular machine learning algorithms:

K-Nearest Neighbors (KNN)

Decision Tree (DT)

Support Vector Machine (SVM)

It compares model performance, visualizes the decision tree, and demonstrates predictions on new emails.

🗂 Dataset

Source: Kaggle / UCI Email Spam Detection dataset

Columns:

label → 'ham' or 'spam'

text → content of the email

Preprocessing steps:

Labels converted to numeric (ham = 0, spam = 1)

Text converted to numerical features using TF-IDF Vectorization

🛠 Approach & Models
1️⃣ K-Nearest Neighbors (KNN)

Predicts an email’s label based on the labels of its nearest neighbors.

Simple and intuitive but can be slower on large datasets.

2️⃣ Decision Tree (DT)

Builds a tree of rules to classify spam vs. ham.

Includes a decision tree visualization for interpretation.


3️⃣ Support Vector Machine (SVM)

Finds the hyperplane that best separates spam from ham in high-dimensional space.

Works well with sparse text features.

📊 Evaluation

Metrics calculated: Accuracy, Precision, Recall, F1-score

Confusion matrices created for each model

Example Confusion Matrix (Decision Tree):


⚡ Example Predictions
Email Text	Prediction
"You won a free ticket!"	Spam
"Are we meeting today?"	Ham
💻 How to Run

Clone the repository:

git clone <your-repo-url>
cd email-spam-detection


Install required packages:

pip install -r requirements.txt


Run the main script or notebook:

python spam_detection.py


The script will:

Preprocess the data

Train KNN, DT, and SVM models

Evaluate metrics and print results

Display confusion matrices

Visualize the decision tree

Predict new email examples

📂 Deliverables

Trained models (.joblib files)

Decision tree visualization (decision_tree.png)

Model comparison table (model_comparison_metrics.csv)

Confusion matrices & classification reports

Demo on new emails

📝 Author

Shivam Singh – BSc Data Science Student
