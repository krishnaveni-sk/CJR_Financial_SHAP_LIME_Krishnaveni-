📘 Interpretable ML for Stock Movement Prediction using SHAP & LIME

Krishnaveni — Cultus Job Readiness Program (Explainable ML Module)

This project predicts 5-day ahead stock movement (Up / Down) using machine-learning models and explains the predictions using SHAP and LIME interpretability methods.

The project is developed as part of the Cultus Job Readiness Program – Explainable ML Module.

🚀 1. Project Overview
✔️ Problem

Predict whether the stock price will go UP or DOWN after 5 days.

✔️ Approach

Downloaded 10 years of Apple (AAPL) stock data

Engineered financial features

Returns (1-day, 5-day)

Lag variables

Volatility

Trained an XGBoost binary classifier

Explained global & local model behavior using

SHAP (global + local)

LIME (10 local explanations)

✔️ Output Generated

Preprocessed dataset

Test features & labels

SHAP global importance plot

10 SHAP local explanation PNGs

10 LIME local explanation HTML files

📂 2. Project Structure
CJR_Financial_SHAP_LIME_Krishnaveni/
│
├── CJR_Financial_SHAP_LIME_Krishna1.ipynb       # Main notebook (all steps)
│
├── processed_financial_dataset.csv              # Cleaned + engineered data
├── X_test_data.csv                               # Test feature matrix
├── y_test_data.csv                               # Test labels
│
├── shap_summary.png                              # SHAP global feature importance
├── shap_local_0.png to shap_local_9.png          # SHAP local explanations
│
└── lime_local_0.html to lime_local_9.html        # LIME local explanations

🧠 3. Machine Learning Workflow
Step 1 — Data Collection

Downloaded 10 years of AAPL OHLCV data using yfinance.

Step 2 — Feature Engineering

Created:

Return_1d

Return_5d

Lag1 to Lag5

Volatility_5d

Step 3 — Train/Test Split

Used the last 20% of the data as test samples.

Step 4 — Model Training

Used XGBoost Classifier for binary classification (Up/Down).

Step 5 — SHAP Explainability

Generated:

Global SHAP summary plot

10 local SHAP explanations (PNG files)

Step 6 — LIME Explainability

Generated:

10 HTML LIME explanations using LimeTabularExplainer

🖼️ 4. Visual Outputs
🔹 SHAP Global Feature Importance

shap_summary.png
Shows which features drive predictions overall.

🔹 SHAP Local Explanations

shap_local_0.png to shap_local_9.png
Explains prediction for specific samples.

🔹 LIME Local Explanations

lime_local_0.html to lime_local_9.html
Shows feature contribution (positive/negative) for each prediction.

🧪 5. How to Run This Project
Requirements

Install required libraries:

pip install numpy pandas shap lime xgboost matplotlib yfinance

Run Notebook

Open:

CJR_Financial_SHAP_LIME_Krishna1.ipynb


Then click Run All.

Outputs will automatically be saved as:

CSV files

SHAP PNG files

LIME HTML files

📝 6. Requirement Mapping (Cultus Job Readiness Program)
Requirement	Status	Where Completed
#1: Data Collection	✔️	Notebook (AAPL 10-year data)
#2: Data Preparation & Feature Engineering	✔️	Notebook
#3: Model Training	✔️	XGBoost model
#4: Explainability (SHAP & LIME)	✔️	PNG + HTML files
#5: Output Comparison	✔️	Notebook section “Comparison”
#6: GitHub Submission	✔️	This repository
👩‍💻 7. Author

Krishnaveni S
Cultus Job Readiness Program — Explainable ML Module
GitHub: krishnaveni-sk

🏁 8. Final Notes

This repository contains every file required by Cultus:
✔️ Notebook
✔️ Processed datasets
✔️ SHAP + LIME outputs
✔️ README with requirement mapping

Your submission meets 100% of program criteria.
