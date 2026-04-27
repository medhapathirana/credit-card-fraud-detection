# Credit Card Fraud Detection

## Overview
This project applies three machine learning models to detect fraudulent 
credit card transactions using the Kaggle Credit Card Fraud Detection dataset.

## Models Used
| Model | F1 Score | AUC-ROC |
|-------|----------|---------|
| Logistic Regression | 0.73 | 0.94 |
| Decision Tree | 0.76 | 0.88 |
| **Random Forest (Best)** | **0.87** | **0.95** |

## Project Structure
- `credit_card_fraud_detection.ipynb` — full ML pipeline (EDA, training, evaluation)
- `app.py` — Streamlit web app for live fraud prediction

## Dataset
Download the dataset from Kaggle and place it in the project root:  
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

## How to Run

### 1. Install dependencies
pip install -r requirements.txt

### 2. Run the notebook
Open `credit_card_fraud_detection.ipynb` in Jupyter and run all cells.  
This generates `fraud_model.pkl` and `scaler.pkl`.

### 3. Run the Streamlit app
streamlit run app.py

## Results
Random Forest achieved the best performance:
- Accuracy: 99.8%
- Precision: 0.94
- Recall: 0.82
- F1 Score: 0.87
- AUC-ROC: 0.95
