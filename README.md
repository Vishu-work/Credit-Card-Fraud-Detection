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

credit-card-fraud-detector/
│
├── creditcard.csv # Dataset file
├── train_model.py # Script to train and save model
├── app.py # Gradio app script
├── model.pkl # Saved logistic regression model
├── scaler.pkl # Saved StandardScaler
├── requirements.txt # Dependencies
└── README.md

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

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/credit-card-fraud-detector.git
cd credit-card-fraud-detector
