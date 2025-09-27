# 📧 Email Spam Detection

## Overview
Classifies emails as **spam** or **ham** using three machine learning algorithms:  

- K-Nearest Neighbors (KNN)  
- Decision Tree (DT)  
- Support Vector Machine (SVM)  

Includes model evaluation, confusion matrices, and decision tree visualization.

---

## Dataset
- Source: Kaggle / UCI Email Spam Detection  
- Columns: `label` (ham/spam), `text` (email content)  
- Labels converted to numeric (`ham = 0`, `spam = 1`)  
- Text converted to numeric features using **TF-IDF**  

---

## Usage
```bash
git clone <your-repo-url>
cd email-spam-detection
pip install -r requirements.txt
python spam_detection.py
