 Customer Churn Prediction App

## Overview

This Streamlit app predicts customer churn probability using a pre-trained TensorFlow model. It processes user inputs, applies necessary preprocessing, and displays churn likelihood dynamically.

## Features

- **User-Friendly Interface**: Input key customer attributes like geography, gender, age, balance, credit score, etc.
- **Preprocessing**: Automated encoding and scaling of inputs.
- **Churn Prediction**: Uses a trained deep learning model to estimate churn probability.
- **Real-Time Insights**: Displays churn likelihood and actionable feedback.

## Setup Instructions

1. Clone the repository.
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Place the following files in the project directory:
   - `model.h5`: Trained TensorFlow model.
   - `label_encoder_gender.pkl`: Gender label encoder.
   - `onehot_encoder_geo.pkl`: Geography one-hot encoder.
   - `scaler.pkl`: StandardScaler for input scaling.
4. Run the app:
   ```bash
   streamlit run app.py
   ```

## How to Use

1. **Provide Customer Details**: Fill in the fields like geography, gender, age, balance, and others.
2. **View Prediction**: The app calculates and displays the churn probability and a corresponding recommendation.

## Dependencies

- **TensorFlow**
- **Streamlit**
- **Scikit-learn**
- **Pandas**
- **Pickle**

## Example Input

- Geography: `France`
- Gender: `Female`
- Age: `30`
- Balance: `1200.50`
- Credit Score: `750`
- Estimated Salary: `50000`
- Tenure: `5`
- Number of Products: `2`
- Has Credit Card: `1`
- Is Active Member: `1`

---

**Output**:  
Churn Probability: `0.67`  
**The customer is likely to churn.**

---

Make smarter retention decisions with this app! 😊
