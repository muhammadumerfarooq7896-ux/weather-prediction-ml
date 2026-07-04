# 🌦️ Weather Prediction Using Machine Learning

## 📌 Project Overview

This project predicts whether it will rain the next day (`RainTomorrow`) using historical Australian weather data and multiple machine learning algorithms. The project demonstrates a complete end-to-end machine learning workflow, including data preprocessing, exploratory data analysis, feature engineering, hyperparameter tuning, model evaluation, and performance comparison.

The objective was to identify the best-performing model for rainfall prediction while following industry-standard machine learning practices.

---

## 📂 Dataset

**Dataset:** Australian Weather Dataset (`weatherAUS.csv`)

The dataset contains daily weather observations collected from multiple locations across Australia. Features include:

* Temperature
* Rainfall
* Humidity
* Pressure
* Wind Speed
* Wind Direction
* Sunshine
* Cloud Cover
* Evaporation
* And several other meteorological variables

**Target Variable**

* `RainTomorrow`

  * 1 = Rain
  * 0 = No Rain

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* LightGBM

---

## 📊 Project Workflow

### 1. Data Preprocessing

* Removed unnecessary columns
* Handled missing values
* Encoded categorical variables
* Scaled numerical features (for Logistic Regression)
* Addressed class imbalance using `class_weight="balanced"`
* Split the dataset into training and testing sets

---

### 2. Exploratory Data Analysis (EDA)

Performed exploratory analysis using various visualizations including:

* Histograms
* Correlation heatmap
* Target class distribution
* Feature distributions

---

### 3. Machine Learning Models

Three different classification models were implemented and compared.

### Logistic Regression

* Hyperparameter tuning using GridSearchCV
* Cross-validation
* ROC Curve
* Precision-Recall Curve
* Confusion Matrix

---

### Random Forest

* Hyperparameter tuning using GridSearchCV
* Cross-validation
* ROC Curve
* Precision-Recall Curve
* Confusion Matrix

---

### LightGBM

* Hyperparameter tuning using GridSearchCV
* Cross-validation
* ROC Curve
* Precision-Recall Curve
* Confusion Matrix

---

## 📈 Model Performance

| Model               |   F1 Score |    ROC-AUC |     PR-AUC |
| ------------------- | ---------: | ---------: | ---------: |
| Logistic Regression |     0.6130 |     0.8625 |     0.6867 |
| Random Forest       |     0.6376 |     0.8753 |     0.7108 |
| **LightGBM**        | **0.6436** | **0.8878** | **0.7372** |

---

## 🏆 Best Model

LightGBM achieved the highest performance across all evaluation metrics.

* **F1 Score:** 0.6436
* **ROC-AUC:** 0.8878
* **PR-AUC:** 0.7372

Based on these results, LightGBM was selected as the final model for rainfall prediction.

---

## 📷 Generated Visualizations

The project includes:

* Feature histograms
* Correlation heatmap
* Confusion matrices
* ROC curves
* Precision-Recall curves

for each machine learning model.

---

## 📁 Repository Structure

```text
Weather-Prediction-ML/
│
├── weather_prediction.ipynb
├── weatherAUS.csv
├── README.md
│
├── images/
│   ├── logreg_confusion_matrix.png
│   ├── logreg_roc_curve.png
│   ├── logreg_pr_curve.png
│   ├── rf_confusion_matrix.png
│   ├── rf_roc_curve.png
│   ├── rf_pr_curve.png
│   ├── lgbm_confusion_matrix.png
│   ├── lgbm_roc_curve.png
│   └── lgbm_pr_curve.png
```

---

## 🚀 Future Improvements

Possible improvements include:

* Feature engineering
* Threshold optimization
* RandomizedSearchCV or Bayesian optimization
* XGBoost comparison
* CatBoost comparison
* Model explainability using SHAP
* Deployment using Streamlit or Flask

---

## 🎯 Key Skills Demonstrated

* Data Cleaning
* Data Preprocessing
* Exploratory Data Analysis
* Feature Engineering
* Machine Learning
* Classification
* Hyperparameter Tuning
* Cross Validation
* Model Evaluation
* Data Visualization
* Python Programming
* Scikit-learn
* LightGBM

---

## 📜 License

This project is intended for educational and portfolio purposes.
