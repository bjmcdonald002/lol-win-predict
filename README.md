# League of Legends Win Prediction

Binary classification of match outcomes in *League of Legends* using structured post-game statistics from ranked solo/duo matches.

## 📊 Project Overview

I trained and compared several models to predict whether a team won or lost based on numeric stat lines and selected the highest-performing models for the data:

- **XGBoost**
- **LightGBM**
- **L1-regularized Logistic Regression**
- **L2-regularized Logistic Regression**
- **Neural Network (MLPClassifier)**

Each model was evaluated with:
- Accuracy, F1 Score, ROC AUC  
- **k-fold cross-validation**  
- **Shuffle testing** (label permutation)

## 📂 Dataset

Publicly available on Kaggle:

🔗 [League of Legends Match Dataset (2025) – Jakub Krasuski](https://www.kaggle.com/datasets/jakubkrasuski/league-of-legends-match-dataset-2025)

## 🔍 Methods & Features

- Cleaned and scaled gameplay data from **21 K+** ranked matches
- Ensemble methods peform best, likely due to capturing non-linear interactions
- Rigorous validation (k-fold CV + shuffle tests)

## 📁 Files

- `binary_class_models_comparison.ipynb` — Comparison of several binary classification models
- `PCLR_league_data.ipynb` - Manual robust PCA implementation with Logistic Regression for exploratory modeling and comparison
- `binary_class_neural_network_league_data.ipynb` — MLP with grid search on an alternative feature set for exploratory modeling and comparison

## 💡 Key Result

> **LightGBM** achieved the highest ROC AUC (~0.966), edging out **XGBoost** (~0.965).  

## 🛠 Tools Used
Python (NumPy, pandas, scikit-learn, XGBoost, LightGBM) · TensorFlow/Keras (for MLP) · Matplotlib · Seaborn

## 📄 Related Materials
Findings will appear in a forthcoming research article.

## 👽 Author
*Barrett James McDonald — Ph.D. Student, University of South Florida*

---

Questions or feedback? Feel free to reach out or open an issue.
