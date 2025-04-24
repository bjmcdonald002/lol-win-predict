# League of Legends Win Prediction

This project explores binary classification of match outcomes in *League of Legends* using structured post-game statistics from ranked solo/duo matches.

## 📊 Project Overview

I've trained and compared multiple models to predict whether a match resulted in a win or loss based on numeric stat lines. Techniques included:

- **XGBoost**
- **LightGBM**
- **L1-regularized Logistic Regression**
- **Neural Network (MLPClassifier)**
- **Principal Component Logistic Regression (with robust PCA)**

Each model was evaluated using:
- Accuracy, F1 Score, ROC AUC
- K-Fold Cross-Validation
- Shuffle Testing (label permutation)

## 📂 Dataset

The dataset used in this project is publicly available on Kaggle:

🔗 [League of Legends Match Dataset (2025) – by Jakub Krasuski](https://www.kaggle.com/datasets/jakubkrasuski/league-of-legends-match-dataset-2025)

## 🔍 Methods & Features

- Applied **robust PCA** via low-rank decomposition
- Used ensemble methods to capture non-linear interactions
- Validated results with **statistical rigor**
- Cleaned and scaled gameplay data from over 21,000 ranked matches

## 📁 Files

- `binary_class_models.ipynb` — Exploratory modeling and comparison
- `PCLR_league_data.ipynb` — Manual robust PCA implementation with Logistic Regression
- `binary_class_neural_network_league_data.ipynb` - Multi-Layer Neural Network implementing a grid search, different feature set than other projects

## 💡 Key Result

> XGBoost achieved the highest ROC AUC (0.9650), followed closely by LightGBM (0.9638). Logistic regression with robust PCA provided strong theoretical grounding with ROC AUC 0.9076.

## 🛠 Tools Used

- Python (NumPy, pandas, scikit-learn, XGBoost, LightGBM)
- Matplotlib / Seaborn for plots
- LaTeX for reporting

## 📄 Related Materials

This project is featured in a forthcoming research article.

## 👽 Author

*Prepared by Barrett James McDonald | PhD Student | University of South Florida*

---

If you have any questions or feedback, feel free to contact me or open an issue. 💬
