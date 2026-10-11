# Smart Loan Eligibility and Default Risk Prediction System

An interactive loan analysis project combining a web frontend, a FastAPI backend, a machine-learning prediction pipeline, financial risk scoring, and personalized recommendations.

## Project Components

- `frontend/` — HTML, CSS, and JavaScript interface
- `backend/` — FastAPI endpoints and request schemas
- `src/` — prediction pipeline, feature engineering, preprocessing, risk analysis, and recommendations
- `data/raw/Loan.csv` — project dataset used for analysis/training
- `models/loan_approval_model.pkl` — trained model used by the prediction pipeline
- `eda/outputs/` — exploratory data analysis charts and summaries
- `training/` — model training and feature experiments
- `Smart_loan_Risk_Prediction(presentation).pptx` — project presentation

## Requirements

The backend dependencies are listed in `backend/requirements.txt`.

## Run Locally

Run commands from the project root directory.

1. Create and activate a Python virtual environment (recommended).
2. Install dependencies:

   ```bash
   pip install -r backend/requirements.txt
   ```

3. Start the API:

   ```bash
   uvicorn backend.main:app --reload
   ```

4. Open the API documentation at `http://127.0.0.1:8000/docs`.

The frontend files are in `frontend/`. The frontend's API connection settings may need to be configured for the address where the backend is running.

## Important Notes

- This project is for educational and demonstration purposes only, not for making real lending decisions.
- Model predictions and risk scores depend on the training data and project logic; they should not be treated as financial advice.
- The trained model is included in this repository. If you replace or retrain it, ensure the new model uses the same feature preparation expected by `src/prediction_pipeline.py`.
