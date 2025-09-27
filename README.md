# Email_Spam_Detection
Email Spam Detection Project
📄 Project Overview

This project demonstrates email spam detection using three popular classification algorithms:

K-Nearest Neighbors (KNN)

Decision Tree (DT)

Support Vector Machine (SVM)

The goal is to build models that can classify emails as spam or ham (not spam) and compare their performance using accuracy, precision, recall, and confusion matrices.

🗂 Dataset

The project uses the Email Spam Detection dataset (from Kaggle / UCI repository).

Each email has two columns:

label: 'ham' or 'spam'

text: the email content

Data preprocessing:

Labels are converted to numeric values (ham = 0, spam = 1).

Text is converted to numeric features using TF-IDF Vectorization.

⚙️ Features & Models
1. K-Nearest Neighbors (KNN)

Classifies emails based on labels of nearest neighbors in feature space.

2. Decision Tree (DT)

Splits data using important words to separate spam from ham.

Includes a decision tree visualization for interpretation.

3. Support Vector Machine (SVM)

Finds the hyperplane that best separates spam and ham emails.

Works well on high-dimensional text data.

🛠 Installation & Usage

Clone the repository:

git clone <your-repo-url>
cd email-spam-detection


Install required Python packages:

pip install -r requirements.txt


Run the main notebook or script:

python spam_detection.py


The code will:

Preprocess data with TF-IDF

Train KNN, Decision Tree, and SVM models

Evaluate models with accuracy, precision, recall, and confusion matrices

Visualize the decision tree

Test new example emails

📊 Outputs

Metrics Table: Comparison of accuracy, precision, recall for all models.

Confusion Matrices: For KNN, DT, and SVM.

Decision Tree Visualization: Shows which words are important for classification.

Demo: Predictions on new sample emails.

📝 Example Predictions
"You won a free ticket!" → Predicted: Spam  
"Are we meeting today?" → Predicted: Ham

🔍 How to Interpret

Accuracy: How often the model predicts correctly.

Precision: How many predicted spam emails were actually spam.

Recall: How many actual spam emails were correctly detected.

Decision Tree: Visualizes rules learned from the dataset.

📂 Project Files

spam_detection.py / assignment.ipynb – main code

spam.csv – dataset (not included in GitHub for privacy)

decision_tree.png – decision tree visualization

model_comparison_metrics.csv – metrics table

README.md – project description

📌 Notes

The models are trained on 80% of the dataset and tested on 20%.

TF-IDF is limited to top 1000 words for simplicity.

Decision Tree max depth is limited to 5 for readability.

⚡ Author

Shivam Singh – BSc Data Science Student
