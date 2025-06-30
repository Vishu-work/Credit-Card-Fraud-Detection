# 💳 Credit Card Fraud Detection using Logistic Regression & Gradio

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Model](https://img.shields.io/badge/Model-Logistic%20Regression-brightgreen)
![Gradio](https://img.shields.io/badge/UI-Gradio-blueviolet)
![Status](https://img.shields.io/badge/Project-Completed-success)

> 🛡️ Detect fraudulent credit card transactions using machine learning — with a clean, interactive Gradio UI!

---

## 🗂️ Table of Contents

- [📖 Overview](#-overview)
- [📦 Features](#-features)
- [🧠 How It Works](#-how-it-works)
- [🖥️ Gradio Interface](#️-gradio-interface)
- [🚀 Getting Started](#-getting-started)
- [📊 Dataset Info](#-dataset-info)
- [📸 Sample UI](#-sample-ui)
- [🔮 Future Enhancements](#-future-enhancements)
- [🙌 Acknowledgements](#-acknowledgements)
- [📬 Contact](#-contact)

---

## 📖 Overview

This project builds a **fraud detection system** using the popular `creditcard.csv` dataset from Kaggle.  
The model is trained using **Logistic Regression** and deployed via **Gradio** for an intuitive user interface to predict whether a credit card transaction is **fraudulent or not**.

🧠 Built using:
- Python
- Pandas, scikit-learn
- Logistic Regression
- Gradio

---

## 📦 Features

✅ Predicts if a transaction is **Fraudulent** or **Not Fraudulent**  
✅ Uses **StandardScaler** to normalize input features  
✅ Handles **imbalanced data** using `class_weight="balanced"`  
✅ Evaluation using Accuracy, Precision, Recall, F1-score  
✅ Clean and interactive **Gradio interface**  
✅ Exception handling for invalid or missing inputs

---

## 🧠 How It Works

```mermaid
graph LR
A[creditcard.csv Dataset] --> B[Data Preprocessing & Scaling]
B --> C[Train-Test Split]
C --> D[Model Training - Logistic Regression]
D --> E[Model Evaluation - Metrics]
E --> F[Model Saving - model.pkl & scaler.pkl]
F --> G[Gradio Web App for Prediction]
