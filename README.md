📧 Email Spam Detection: A Comparative Study
Project Overview
This project implements and compares three powerful machine learning classifiers—K-Nearest Neighbors (KNN), Decision Tree (DT), and Support Vector Machine (SVM)—to accurately classify emails as spam or ham (not spam). The primary goal is to evaluate their performance using key metrics like accuracy, precision, and recall, providing a comprehensive view of which algorithm is most effective for this task.

🚀 Key Features
Comparative Analysis: Performance metrics (Accuracy, Precision, Recall) are generated for all three models.

Feature Engineering: Utilizes TF-IDF Vectorization for converting raw email text into meaningful numerical features.

Model Interpretability: Includes a visualization of the Decision Tree to illustrate the learned classification rules.

Robust Evaluation: Generates Confusion Matrices for a detailed breakdown of model errors.

Live Demo: Demonstrates predictions on new, unseen email examples.

🗂 Dataset
The project utilizes a well-known Email Spam Detection dataset (often sourced from Kaggle or the UCI repository).

Column	Description
label	Classification: 'ham' or 'spam'
text	The full content of the email

Export to Sheets
Data Preprocessing Notes:
Label Encoding: ham is converted to 0 and spam is converted to 1.

Feature Vectorization: The email text is converted into a numeric feature set using TF-IDF (Term Frequency-Inverse Document Frequency).

Note: For simplicity and efficiency, TF-IDF is limited to the top 1000 most frequent words.

Train-Test Split: Models are trained on 80% of the data and tested on the remaining 20%.

⚙️ Model Implementations
1. K-Nearest Neighbors (KNN)
Classifies a new email based on the majority label of its closest neighbors in the feature space. A simple yet effective non-parametric method.

2. Decision Tree (DT)
A white-box model that builds a tree structure by splitting the data based on the most important words that help separate spam from ham.

Note: The tree depth is limited to 5 for optimal readability and interpretation.

3. Support Vector Machine (SVM)
Finds the optimal hyperplane that maximizes the margin between the spam and ham classes. It is particularly effective for high-dimensional text data.

🛠 Installation and Usage
Prerequisites
Python 3.x

The spam.csv dataset (must be placed in the project directory)

Steps
Clone the Repository:

Bash

git clone <your-repo-url>
cd email-spam-detection
Install Dependencies:

Install all required Python packages using the provided requirements.txt file.

Bash

pip install -r requirements.txt
Run the Project:

Execute the main script/notebook to perform data preprocessing, model training, evaluation, and generate outputs.

Bash

python spam_detection.py
# OR open and run the assignment.ipynb notebook
📊 Outputs and Interpretation
Metrics Comparison Table
A generated model_comparison_metrics.csv will provide a clear, side-by-side view of model performance.

Metric	Interpretation	Importance in Spam Detection
Accuracy	Overall correctness: (True Positives+True Negatives)/Total	General measure of model performance.
Precision	Out of all emails predicted as SPAM, how many were actually SPAM?	Crucial for minimizing False Positives (important email marked as spam).
Recall	Out of all actual SPAM emails, how many were correctly detected?	Crucial for minimizing False Negatives (spam email getting to the inbox).

Export to Sheets
Confusion Matrices
A visual breakdown (for KNN, DT, and SVM) showing True Positives, True Negatives, False Positives, and False Negatives.

Decision Tree Visualization
The decision_tree.png file provides a visual roadmap of the rules learned by the Decision Tree model, highlighting the most informative words.

📝 Example Predictions
Email Text	Predicted Label
"You won a free ticket! Claim now."	Spam
"Are we meeting today at the office?"	Ham

Export to Sheets
📂 Project Files Structure
email-spam-detection/
├── spam_detection.py / assignment.ipynb   # Main code (preprocessing, training, evaluation)
├── requirements.txt                       # List of dependencies
├── decision_tree.png                      # Visualization of the Decision Tree model
├── model_comparison_metrics.csv           # Model performance metrics table
├── spam.csv                               # The dataset (required to run the project)
└── README.md                              # This file
⚡ Author
Shivam Singh – BSc Data Science Student

Feel free to connect or contribute!
