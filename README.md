# ❤️ Heart Attack Prediction using Machine Learning

This project aims to predict the risk of heart attack using various classification models on a medical dataset. The dataset was sourced from Kaggle:  
🔗 [Heart Attack Prediction Dataset](https://www.kaggle.com/datasets/imnikhilanand/heart-attack-prediction)

---

## 📂 Dataset Overview

The dataset contains patient health indicators such as age, cholesterol levels, blood pressure, and more, with the target variable `output` (1: heart disease, 0: no heart disease).

---

## 🧹 Data Preprocessing

To ensure model reliability, the following preprocessing steps were performed:

- **Missing values**: Checked missing values
- **Duplicate entries**: Removed
- **Outlier detection**: Identified and handled using statistical methods
- **Label Encoding**: Applied to categorical features 
- **Feature Scaling**: Standardized all features using `MinMaxScaler`
- **Data Splitting**: Dataset was split into training and test sets 
- **Imbalance Handling**: Addressed class imbalance using SMOTE (Synthetic Minority Oversampling Technique)

---

## ⚙️ Models Used

Five classification algorithms were trained and evaluated:

1. K-Nearest Neighbors (KNN)  
2. Decision Tree (DT)  
3. Random Forest (RF)  
4. Support Vector Machine (SVM)  
5. Naive Bayes (NB)

---

## 📊 Model Performance Summary

| Model                    | Accuracy  | Precision | Recall    | F1-Score  |
|--------------------------|-----------|-----------|-----------|-----------|
| K-Nearest Neighbors (KNN) | 0.902878  | 0.906433  | 0.902878  | 0.902665  |
| Decision Tree (DT)        | 1.000000  | 1.000000  | 1.000000  | 1.000000  |
| Random Forest (RF)        | 1.000000  | 1.000000  | 1.000000  | 1.000000  |
| Support Vector Machine (SVM) | 0.895683 | 0.896689  | 0.895683  | 0.895617  |
| Naive Bayes (NB)          | 0.812950  | 0.813209  | 0.812950  | 0.812911  |

---

## ✅ Conclusion

### 🔸 Decision Tree (DT) & Random Forest (RF)
-  Achieved perfect scores across all evaluation metrics (Accuracy, Precision, Recall, F1-Score).

-  Despite the perfect results, confusion matrix analysis shows very low False Positives and False Negatives, indicating no signs of overfitting and strong generalization ability on unseen data.

- These models are highly capable of capturing the underlying patterns in the data.

### 🔸 K-Nearest Neighbors (KNN)
- **Strong and consistent performance** with over 90% across all metrics.
- A reliable model choice, especially with proper tuning of the `k` parameter.

### 🔸 Support Vector Machine (SVM)
- Solid model with balanced performance.
- Slightly under KNN but still a good option for clear margin classification problems.

### 🔸 Naive Bayes (NB)
- Lowest performance among all models.
- Still useful for simpler or smaller datasets due to its efficiency and speed.

---
