# Heart Disease Prediction ❤️🩺

## Background
Early detection of heart disease can help reduce severe outcomes. This project uses machine learning to predict the risk of heart disease based on patient features.

---

## Dataset
**Heart Failure Prediction dataset** (Kaggle, FEDESORIANO)  
- 918 records  
- 11 features + 1 target (`HeartDisease`)  
- [Download from Kaggle](https://www.kaggle.com/fedesoriano/heart-failure-prediction)
  ⚠️ Dataset is not included in this repository due to Kaggle license.  
Please download it directly from Kaggle if you want to reproduce the results.

---

## Folder Structure
```
heart-disease-ml/
├── notebooks/ Jupyter notebooks (EDA, training, evaluation)
├── models/ Saved KNN model (knn_heart_disease.joblib)
├── data/ Dataset CSV (not included, download from Kaggle)
├── requirements.txt Python libraries used
├── README.md
```
---

## Example Results

### 1. Data Distribution
![data_distribution](images/data_distribution.png)

### 2. Correlation Heatmap
![correlation_heatmap](images/correlation_heatmap.png)

### 3. ROC Curve of KNN Model
![roc_curve](images/roc_curve.png)

---

## Models & Evaluation
| Model | F1-score | Precision | Recall |
|-------|---------|----------|-----------|
| KNN     | 0.8161     | 0.870      | 0.853   |

> For full details on exploratory data analysis, feature engineering, and model evaluation, see the notebook in `notebooks/`.

---

## Usage
```python
from joblib import load

# Load trained model
knn_model = load("models/knn_heart_disease.joblib")

# Predict on new data
predictions = knn_model.predict(X_new)
```

---

## Dependencies
Required Python libraries are listed in `requirements.txt`.  
Install them using:

```bash
pip install -r requirements.txt
```
---

## Notes
- Interactive plots (e.g., correlation heatmap) are available on [Kaggle Notebook](https://www.kaggle.com/code/enfantksr/heartdisease-prediction)
