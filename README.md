# customer-churn-prediction
This project predicts whether a bank customer will leave the bank (churn) using an Artificial Neural Network (ANN) built with TensorFlow/Keras.
The dataset contains information such as geography, credit score, age, balance, and more.
The goal is to help banks identify at-risk customers and take action to improve retention.
📊 Dataset

Source: Kaggle – Bank Customer Churn Modeling

Rows: 10,000 bank customers

Target: Exited (1 = customer left, 0 = customer stayed)

Key features include:

Geography, Gender, Credit Score, Age, Balance, Products, Credit Card, Active Member, Estimated Salary, etc.

***************************************************************************************************************************

# 🧠 Model Overview

Input Preprocessing

Label Encoding for Gender

One-Hot Encoding for Geography

Standardization using StandardScaler

Model Architecture

Input layer: Encoded features

2 Hidden layers: 6 neurons each, ReLU activation

Output layer: 1 neuron, Sigmoid activation

Training

Optimizer: Adam

Loss: binary_crossentropy

Epochs: 100

Batch size: 32

***************************************************************************************************************************

# 🚀 How to Run

Clone this repository:

git clone https://github.com/yourusername/customer-churn-prediction.git
cd customer-churn-prediction

Run the notebook:
jupyter notebook churn_ann.ipynb


or run the Python script:
python churn_ann.py

***************************************************************************************************************************

# 📈 Results

Accuracy on Test Set: ~XX% (replace with your actual test accuracy)

Confusion Matrix shows the distribution of correct vs. incorrect predictions.

🔮 Single Prediction Example

You can predict a single customer’s churn probability using:

ann.predict(sc.transform([[1, 0, 0, 600, 1, 40, 3, 60000, 2, 1, 1, 50000]])) > 0.5


This example predicts whether a 40-year-old male customer in France with specific account details will leave the bank.
