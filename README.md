# 📧 Email Spam Detection

## 📄 Project Overview
This project demonstrates **email spam detection** using three popular classification algorithms:

- **K-Nearest Neighbors (KNN)**
- **Decision Tree (DT)**
- **Support Vector Machine (SVM)**

The goal is to build models that classify emails as **spam** or **ham** and compare their performance using **accuracy, precision, recall**, and **confusion matrices**.

---

## 🗂 Dataset
- **Source:** Kaggle / UCI Email Spam Detection dataset  
- **Columns:**
  - `label` → 'ham' or 'spam'  
  - `text` → email content  

**Preprocessing Steps:**
- Convert labels to numeric (`ham = 0`, `spam = 1`)  
- Convert text to numeric features using **TF-IDF Vectorization**

---

## ⚙️ Models & Approach

### 1️⃣ K-Nearest Neighbors (KNN)
- Predicts email labels based on **nearest neighbors** in feature space.

### 2️⃣ Decision Tree (DT)
- Builds a **tree of rules** to classify spam vs. ham  
- Includes **decision tree visualization** to interpret important words

### 3️⃣ Support Vector Machine (SVM)
- Finds a **hyperplane** that separates spam and ham in high-dimensional feature space  
- Performs well on text data with many features

---

## 🛠 Installation & Usage

1. Clone the repository:
```bash
git clone <your-repo-url>
cd email-spam-detection
