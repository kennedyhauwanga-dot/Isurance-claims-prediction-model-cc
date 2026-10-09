# Insurance Claim Risk Prediction Model

This is a Streamlit web application that predicts the likelihood of an insurance policyholder filing a claim within the next 12 months using an XGBoost machine learning model.

## Features
- **Interactive UI:** Adjust policyholder age, vehicle value, vehicle age, and annual premium in the sidebar.
- **XGBoost Model:** Trained on historical insurance data to output a probability and a binary classification (Claim / No Claim).
- **Risk Levels:** Color-coded Low, Medium, and High risk output.
- **Feature Importance:** Top 15 predictors displayed as a bar chart and table.
- **Prediction Logging:** Each prediction is saved to a local SQLite database (`predictions.db`).

## Dataset
The model uses `insurance_claims.xlsx` (Sheet: `Data_Part_1`). 
*Note: The first time the app runs, it will train the model and save `xgb_12m_model.pkl`. Subsequent runs load the saved model instantly.*

## Local Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Insurance-claims-prediction-model-cc.git
   cd Insurance-claims-prediction-model-cc
