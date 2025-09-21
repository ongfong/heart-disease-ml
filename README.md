# Heart Disease Prediction

## Background
Early detection of heart disease can reduce severe outcomes. Machine learning can help identify patients at risk.

## Dataset
Heart Failure Prediction dataset (Kaggle, FEDESORIANO)  
- 918 records, 11 features + 1 target (`HeartDisease`)

## Folder Structure
- `notebooks/` → Jupyter Notebooks (EDA, training, evaluation)
- `models/` → Saved KNN model (`knn_heart_disease.joblib`)
- `data/` → Dataset (optional, download from [Kaggle Heart Failure Prediction](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction?select=heart.csv))
- `requirements.txt` → Python libraries used

## Usage
```python
from joblib import load
knn_model = load("models/knn_heart_disease.joblib")
predictions = knn_model.predict(X_new)
