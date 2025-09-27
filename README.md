📧 Email Spam Detection
Overview

This project classifies emails as spam or ham using three popular machine learning algorithms:

K-Nearest Neighbors (KNN)

Decision Tree (DT)

Support Vector Machine (SVM)

The goal is to compare model performance and visualize the decision-making process.

Dataset

Source: Email Spam Detection dataset (Kaggle / UCI)

Columns:

label → 'ham' or 'spam'

text → content of the email

Preprocessing:

Labels are converted to numeric: ham = 0, spam = 1

Text is converted to numerical features using TF-IDF Vectorization

Models & Approach
1️⃣ K-Nearest Neighbors (KNN)

Classifies emails based on the labels of the nearest neighbors.

Simple, intuitive, but can be slower with large datasets.

2️⃣ Decision Tree (DT)

Builds a tree of rules to separate spam from ham.

Includes a decision tree visualization for interpretation.

3️⃣ Support Vector Machine (SVM)

Finds a hyperplane that best separates spam and ham in high-dimensional space.

Performs well with text data.

Evaluation

Metrics calculated: Accuracy, Precision, Recall, F1-score

Confusion matrices created for each model

Decision Tree visualized to understand the features used for classification

Usage

Clone the repository:

git clone <your-repo-url>
cd email-spam-detection


Install required packages:

pip install -r requirements.txt


Run the main script or notebook:

python spam_detection.py


The script will:

Preprocess the data

Train KNN, Decision Tree, and SVM models

Evaluate metrics and print results

Display confusion matrices

Visualize the decision tree

Predict new email examples

Example Predictions
Email Text	Prediction
"You won a free ticket!"	Spam
"Are we meeting today?"	Ham
Deliverables

Trained models (optional .joblib files)

Decision tree visualization (decision_tree.png)

Model comparison table (model_comparison_metrics.csv)

Confusion matrices and classification reports

Demo of new email predictions

Author

Shivam Singh – BSc Data Science Student

This version:

Uses sections, bullet points, and tables for readability

Includes emojis lightly for GitHub visual appeal

Looks professional and clean
