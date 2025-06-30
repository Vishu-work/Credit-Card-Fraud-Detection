💳 Credit Card Fraud Detection with Logistic Regression & Gradio
This project builds a fraud detection model using Logistic Regression trained on the popular creditcard.csv dataset. The trained model is deployed using Gradio, allowing for an easy-to-use web interface to predict whether a transaction is fraudulent or not.

📊 Dataset
Source: Kaggle Credit Card Fraud Detection Dataset

Records: 284,807 transactions

Features:

30 input features (V1 to V28, Time, and Amount)

Target: Class (0 = Non-fraudulent, 1 = Fraudulent)

✅ Features
🔍 Detects fraud using Logistic Regression

🧼 Scaled input features using StandardScaler

🧠 Handles highly imbalanced dataset

🧪 Train-test evaluation with accuracy, recall, precision, F1-score

🌐 Interactive web interface using Gradio

🛡️ Includes exception handling for invalid inputs

🗂️ Project Structure
bash
Copy
Edit
credit-card-fraud-detector/
│
├── creditcard.csv              # Dataset file
├── train_model.py              # Model training script
├── app.py                      # Gradio app script
├── model.pkl                   # Trained logistic regression model
├── scaler.pkl                  # Saved StandardScaler
├── requirements.txt
└── README.md
🧠 How It Works
Data Preprocessing

Drop target column and scale features using StandardScaler

Model Training

Use LogisticRegression with class weight adjustments for imbalance

Model Saving

Save the trained model and scaler using joblib

Gradio Deployment

Accept user input through UI and return prediction (Fraud/Not Fraud)

🚀 Getting Started
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/credit-card-fraud-detector.git
cd credit-card-fraud-detector
2. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
3. Train the Model (Optional)
bash
Copy
Edit
python train_model.py
4. Run the Gradio App
bash
Copy
Edit
python app.py
🌐 Gradio Interface
Inputs: 30 features (as numerical inputs, same as V1 to V28, Amount, Time)

Output: "Fraudulent" or "Not Fraudulent"

