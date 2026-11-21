# NovaGen Health Risk Classification 🧬

## 📌 Project Overview

NovaGen Health Risk Classification is a Machine Learning project developed to identify individuals based on their health profiles using physiological measurements, lifestyle factors, and medical history.

The project aims to classify individuals into two categories: **Healthy and Unhealthy**, supporting population health research, participant selection, and risk-based analysis.

Using supervised machine learning algorithms, this project explores how different health indicators can contribute to predicting an individual's health status.

## 🎯 Problem Statement

NovaGen Research Labs conducts large-scale population health studies but requires a consistent approach to distinguish individuals with generally healthy profiles from those potentially at higher health risk.

The objective is to develop a binary classification model that predicts an individual's health category based on available health indicators.

Potential applications include:
- Supporting participant selection for clinical trials.
- Identifying individuals who may require further health assessment.
- Supporting population stratification for research.
- Comparing health outcomes across different population groups.

## 📊 Dataset Description

The dataset contains **9,549 individual health records** with 22 input features and one target variable.

The dataset includes:

| Category | Features |
|---|---|
| Physiological | Age, BMI, Blood Pressure, Cholesterol, Glucose Level, Heart Rate |
| Lifestyle | Sleep Hours, Exercise Hours, Water Intake, Stress Level |
| Behavioral | Smoking, Alcohol, Diet |
| Health Indicators | Mental Health, Physical Activity, Medical History, Allergies |
| Encoded Features | Diet Type and Blood Group |
| Target | Binary health classification |

**Dataset Statistics:**
- Total records: 9,549
- Input features: 22
- Target classes: 2
- Missing values: 0

## ⚙️ Technologies Used

- Python
- Pandas – Data manipulation and analysis
- NumPy – Numerical operations
- Scikit-learn – Machine Learning and model evaluation
- Matplotlib / Seaborn – Data visualization (if used)

## 🧠 Machine Learning Approach

This project follows a supervised machine learning classification approach.

### 1. Data Loading
Loaded the dataset using Pandas and separated the independent features (X) from the target variable (y).

### 2. Train-Test Split
Split the dataset into training and testing sets using an 80:20 ratio.

Stratified sampling was applied to maintain the target class distribution across both sets.

### 3. Data Preprocessing
The preprocessing stage includes:
- Feature scaling using StandardScaler where appropriate.
- Handling numerical and categorical features.
- Preparing data for different classification algorithms.

### 4. Model Development

The following classification algorithms are being explored:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Random Forest Classifier
- Gradient Boosting Classifier
- Voting Classifier (Ensemble Learning)

### 5. Model Evaluation

Models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report

Special attention is given to recall because identifying potentially higher-risk individuals is an important consideration in health-related classification.

## 📈 Results

All models were evaluated on the same stratified test set, and their performance is compared below.

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---|---|---|---|
| Logistic Regression |  0.81  | 0.81 | 0.83 | 0.82 |
| KNN | 0.88 | 0.89 | 0.88 | 0.89 |
| Random Forest | 0.938 | 0.95 | 0.96 | 0.94 |
| Gradient Boosting | 0.93 | 0.94 | 0.95 | 0.93 |
| Voting Classifier | 0.91 | 0.92 | 0.93 | 0.92 |

## 🚀 Future Improvements

- Hyperparameter tuning for improved model performance.
- Feature importance analysis to understand influential health indicators.
- Advanced ensemble learning techniques.
- Model deployment using Streamlit.
- Interactive health-risk prediction interface.

## ⚠️ Disclaimer

This project is developed for educational and research purposes. Predictions should not be considered medical diagnoses or substitutes for professional medical advice.

## 👩‍💻 Author

**Debasmita Sarkar**

GitHub: [Miss-Jojo](https://github.com/Miss-Jojo)
