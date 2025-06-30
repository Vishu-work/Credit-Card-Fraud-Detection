# 💳 Credit Card Fraud Detection using Logistic Regression & Gradio

This project builds a **fraud detection model** using **Logistic Regression**, trained on the widely used **Kaggle Credit Card Fraud Detection Dataset**. The trained model is deployed using **Gradio**, offering an intuitive web interface to predict whether a transaction is fraudulent or not.

---

## 📊 Dataset

- **Source**: [Kaggle - Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Records**: 284,807 transactions
- **Features**:
  - 30 input variables: `V1` to `V28`, `Time`, and `Amount`
  - `Class`: Target variable (`0 = Non-fraudulent`, `1 = Fraudulent`)

---

## ✅ Features

- 🔍 Predicts fraud using **Logistic Regression**
- 📉 Scales input features with `StandardScaler`
- ⚖️ Handles **imbalanced dataset** with class weighting
- 📊 Evaluates model with **accuracy, precision, recall, F1-score**
- 🌐 Deploys model using **Gradio** for a web interface
- 🛡️ Includes **robust exception handling**

---

## 🗂️ Project Structure

📦 credit-card-fraud-detector
├── 📁 data/
│   └── 📄 creditcard.csv         # Original dataset from Kaggle
│
├── 🧠 train_model.py             # Script to clean, train, and save the model
├── 🌐 app.py                     # Gradio UI for making real-time predictions
│
├── 📦 models/
│   ├── model.pkl                 # Saved Logistic Regression model
│   └── scaler.pkl                # Saved StandardScaler instance
│
├── 📄 requirements.txt           # List of Python dependencies
├── 📘 README.md                  # Project documentation (this file)
└── 📄 .gitignore                 # Files to ignore in version control

markdown
Copy
Edit

---

## 🧠 How It Works

### 1. **Data Preprocessing**
- Drop the `Class` column from features
- Scale numerical values using `StandardScaler`

### 2. **Model Training**
- Train a `LogisticRegression` model
- Use `class_weight='balanced'` to manage data imbalance

### 3. **Model Saving**
- Save the trained model and scaler using `joblib`

### 4. **Gradio Deployment**
- Accepts 30 inputs: `V1-V28`, `Amount`, `Time`
- Outputs: `"Fraudulent"` or `"Not Fraudulent"`

---

