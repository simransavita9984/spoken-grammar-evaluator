# 🎙️ Grammar Scoring Engine (Audio-Based ML Project)

A Machine Learning model to evaluate spoken English grammar quality from audio clips using MFCC features and regression algorithms.

---

## 📌 Project Overview

This project aims to predict grammar scores (0-5 scale) based on users' spoken audio. It extracts acoustic features using MFCCs and applies ML models to estimate the grammar quality. Ideal for applications like language learning, automated spoken assessments, and communication skill analysis.

---

## ⚙️ Tech Stack Used

- **Python 3**
- **Librosa** – audio processing & MFCC extraction
- **NumPy, Pandas** – data handling
- **Scikit-learn** – Ridge Regression, Random Forest, metrics
- **XGBoost** – advanced gradient boosting (optional)
- **Joblib** – model saving
- **Jupyter Notebook** – development environment

---

## 📂 Project Structure
GrammarScoringEngine/
├── notebooks/ → main code notebook
├── audios/ → training audio
├── audios_test/ → test audio
├── submission.csv → final output
├── final_grammar_model.pkl → saved model
├── requirements.txt
├── README.md
└── .gitignore

---

## 🧪 Key Steps

1. **Preprocessing**: Converted `.wav` files into MFCC feature vectors.
2. **Model Training**:
   - Tried **Ridge Regression**, **Random Forest**, **XGBoost**.
   - Best results from **Random Forest**:  
     - ✅ *MSE*: `1.17`  
     - ✅ *R² Score*: `0.13`
3. **Prediction**: Extracted MFCC from test audio and predicted scores.
4. **Submission**: Created `submission.csv` with filename & predicted scores.
5. **Model Saved**: Using `joblib` for reuse.

---

## 📈 Results

| Model          | MSE     | R² Score |
|----------------|---------|----------|
| Ridge          | 1.24    | 0.08     |
| Random Forest  | ✅ 1.17 | ✅ 0.13   |
| XGBoost        | 1.37    | -0.00    |

---

