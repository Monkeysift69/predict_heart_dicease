
# Heart Disease Prediction

This project uses the UCI Heart Disease dataset to predict the presence of heart disease using Logistic Regression and scikit-learn.

## 📊 Dataset
- Source: UCI Machine Learning Repository
- Combined multiple `.data` files from Cleveland, Hungarian, Switzerland, and Long Beach datasets.
- Cleaned, encoded, and scaled using standard preprocessing.

The dataset used in this project comes from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/heart+Disease).  
All rights and credit go to the original creators. This repository uses the dataset strictly for educational purposes.

## 🔍 Features
- 13 medical attributes (e.g., age, sex, cp, thalach, chol, ca, thal)
- Target variable: presence of heart disease (1 = disease, 0 = no disease)

## ⚙️ Models Used
- Logistic Regression with `class_weight='balanced'`
- Feature importance plotted from model coefficients
- GridSearchCV for hyperparameter tuning

## 📁 Files Included
- `predict_heart_decease.ipynb`: Jupyter Notebook containing the entire pipeline
- `ridge_model.pkl`: (optional) serialized trained model
- `README.md`: this file

## ✅ Results
- Accuracy > 80% on test set
- Confusion matrix and feature importance visualizations included

## 🧪 How to Use
1. Clone the repository:
```bash
git clone https://github.com/your-username/predict_heart_disease.git
cd predict_heart_disease
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the notebook:
Open `predict_heart_decease.ipynb` and run all cells to reproduce the results.

## 📦 Optional Model Loading
```python
import joblib
model = joblib.load("ridge_model.pkl")
predictions = model.predict(X_test_scaled)
```



**Author**: Rachata Athikamanon  
**License**: MIT
