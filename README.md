# 🧠 Machine Learning–Based Tumor Diagnosis System
## 📌 Overview
This project implements a machine learning–based breast cancer diagnosis system using Support Vector Classification (SVC). The goal is to classify tumors as malignant or benign based on diagnostic features, demonstrating how classical ML models can support medical decision-making.

## 📂 Dataset
* Source: UCI Machine Learning Repository
* Dataset: Breast Cancer Wisconsin (Diagnostic)
* Samples: 569
* Features: 30 numerical diagnostic features
* Target:
    * 0 → Malignant
    * 1 → Benign
The dataset is accessed via scikit-learn to ensure consistency and reproducibility.

## ⚙️ Tech Stack
* Python
* NumPy, Pandas
* Matplotlib, Seaborn
* Scikit-learn

## 🔄 Project Workflow
1. Problem Framing Binary classification to predict tumor malignancy.
2. Exploratory Data Analysis (EDA)
    * Analyzed class distribution
    * Studied feature correlations
    * Identified need for feature scaling
3. Data Preprocessing
    * Train–test split with stratification
    * Applied MinMaxScaler to normalize feature ranges
4. Modeling
    * Used Support Vector Classifier (SVC) with RBF kernel
    * Performed hyperparameter tuning using GridSearchCV
5. Evaluation
    * Metrics: Accuracy, F1-score, Confusion Matrix
    * Focused on reducing false positives while maintaining high recall

## 📊 Results
* Accuracy: ~98%
* F1-score: ~0.96
* Key Outcome: ~25% reduction in false positives compared to an unscaled baseline SVC model

🩺 Interpretation
* Feature scaling significantly improved SVC performance
* Proper metric selection (F1-score) ensured balanced evaluation in a medical context
* The model demonstrates potential as a decision-support system, not a clinical diagnostic tool

## ⚠️ Limitations
* Trained on a relatively small dataset
* No external or clinical validation
* Uses structured diagnostic features only (no imaging data)

## 🚀 Future Improvements
* External dataset validation
* Cost-sensitive learning to further penalize false negatives
