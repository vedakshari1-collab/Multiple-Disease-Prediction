# 🏥 Multiple Disease Prediction System

A machine learning-powered web application that predicts the likelihood of **Diabetes**, **Heart Disease**, and **Parkinson's Disease** from clinical input data — all within a single, unified interface.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=flat-square&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-1.29.0-red?style=flat-square&logo=streamlit)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3.2-orange?style=flat-square&logo=scikit-learn)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

---

## 📌 Overview

This project addresses early disease detection — one of the most critical challenges in preventive healthcare. By training dedicated machine learning models on established clinical datasets and wrapping them in an interactive Streamlit interface, users can input their health parameters and receive an instant prediction for three major diseases.

---

## ✨ Features

- **Multi-Disease Support** — Predict Diabetes, Heart Disease, and Parkinson's Disease from a single application
- **Interactive Web UI** — Clean, responsive interface built with Streamlit and a sidebar navigation menu
- **Pre-Trained ML Models** — Serialised scikit-learn models loaded at runtime for fast, real-time inference
- **Modular Architecture** — Each disease prediction module is independently structured for easy extensibility
- **No Server Required** — Runs entirely locally with a single command

---

## 🧠 Disease Modules

### 🩸 Diabetes Prediction
Predicts whether a patient is diabetic based on 8 clinical features from the **PIMA Indians Diabetes Dataset**, including glucose level, blood pressure, BMI, insulin level, and diabetes pedigree function.

### ❤️ Heart Disease Prediction
Classifies the presence of heart disease using 13 attributes from the **Cleveland Heart Disease Dataset**, including age, chest pain type, resting ECG results, cholesterol levels, and maximum heart rate achieved.

### 🧬 Parkinson's Disease Prediction
Detects Parkinson's Disease from 22 biomedical voice measurements (MDVP features, jitter, shimmer, HNR, RPDE, DFA, etc.) derived from the **UCI Parkinson's Dataset**.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Language | Python 3.8+ |
| Web Framework | Streamlit 1.29.0 |
| ML Library | scikit-learn 1.3.2 |
| Data Processing | NumPy 1.26.3 |
| UI Components | streamlit-option-menu 0.3.6 |
| Model Serialization | Pickle |
| Notebooks | Jupyter |

---

## 📁 Project Structure

```
Multiple-Disease-Prediction/
│
├── app.py                    # Main Streamlit application
├── requirements.txt          # Python dependencies
│
├── data/
    ├── diabetes.csv
    ├── heart.csv
    └── parkinsons.csv                    # Raw datasets for each disease
│
├── notebooks/                   # Jupyter notebooks for model training & evaluation
│    ├── Multiple Disease Prediction- parkinsons
     ├── Multiple disease prediction system - diabetes
     └── Multiple disease prediction system - heart
│
└── models/             # Serialised trained models (.sav)
    ├── diabetes_model.sav
    ├── heart_disease_model.sav
    └── parkinsons_model.sav
```

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- pip

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Sai-Vivek17/Multiple-Disease-Prediction.git
   cd Multiple-Disease-Prediction
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   streamlit run app.py
   ```

4. Open your browser and navigate to `http://localhost:8501`

---

## 🖥️ Usage

1. Use the **sidebar** to select the disease prediction module.
2. Enter the required clinical parameters in the input fields.
3. Click the **prediction button** to get an instant result.
4. The result will be displayed as a success message indicating the predicted health status.

---

## 📊 Model Training

All models were trained in Jupyter Notebooks located in the `models/` directory. The workflow for each model includes:

- Exploratory Data Analysis (EDA)
- Data preprocessing and feature scaling
- Model training using scikit-learn classifiers
- Model evaluation (accuracy, confusion matrix, classification report)
- Serialisation with `pickle` for deployment

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author

**Vedakshari**
[GitHub](https://github.com/vedakshari1-collab)

---

> ⚠️ **Disclaimer:** This application is intended for educational and research purposes only. It is not a substitute for professional medical advice, diagnosis, or treatment. Always consult a qualified healthcare provider.
