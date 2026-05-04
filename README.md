# 🛒 Online Shopper Purchase Prediction

## 📌 Project Overview

This project aims to predict whether a user will make a purchase during an online shopping session using machine learning techniques.

The dataset contains session-level user behavior such as page visits, time spent, bounce rates, and visitor type.

---

## 🎯 Objective

* Build classification models to predict purchase intention
* Handle class imbalance using SMOTE and class weights
* Evaluate models using robust metrics (ROC-AUC, PR-AUC, F1-score)
* Select the best performing model

---

## 📊 Dataset

* Source: Online Shoppers Intention Dataset
* Target Variable: `Revenue` (0 = No Purchase, 1 = Purchase)
* Imbalanced dataset (~84% vs ~16%)

---

## ⚙️ Tech Stack

* Python
* NumPy, Pandas
* Matplotlib, Seaborn
* Scikit-learn
* XGBoost
* Imbalanced-learn (SMOTE)

---

## 🔧 Data Preprocessing

* Removed duplicates
* Feature engineering (Total browsing time)
* One-hot encoding using `get_dummies()`
* Feature scaling using StandardScaler

---

## ⚖️ Handling Class Imbalance

* Applied SMOTE (Synthetic Minority Oversampling)
* Used class weights in models
* Focused on metrics beyond accuracy

---

## 🤖 Models Used

* Logistic Regression
* Random Forest Classifier
* Support Vector Machine (SVM)
* XGBoost Classifier

---

## 📈 Model Performance

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | ~85.6% |
| Precision | ~52%   |
| Recall    | ~82%   |
| F1 Score  | ~64%   |
| ROC-AUC   | ~0.93  |
| PR-AUC    | ~0.72  |

---

## 📊 Key Insights

* High recall ensures most potential buyers are identified
* PageValues is the most important feature
* Random Forest and XGBoost performed best

---

## 📉 Evaluation Techniques

* Train/Validation/Test Split
* Cross-validation
* Confusion Matrix
* ROC Curve
* Learning Curve

---

## 🔍 Feature Importance

Top contributing features:

* PageValues
* ProductRelated_Duration
* Month features
* Informational and Administrative duration

---

## 🧪 Robustness Checks

* Stability across different random seeds
* Feature sensitivity analysis
* Scaling impact analysis

---

## 🚀 Future Improvements

* Hyperparameter tuning with larger search space
* Ensemble models (stacking/blending)
* Deep learning approaches
* Deployment using Flask/Streamlit

---

## 📁 Project Structure

```
├── online_shoppers_intention.csv
├── capstoneproject.ipynb
├── requirements.txt
└── Project Report.pdf
└── README.md
```

---

## ▶️ How to Run

1. Clone the repository:

```
git clone https://github.com/your-username/Online-Shopper-Purchase-Prediction-ML.git
```

2. Install dependencies:

```
pip install -r requirements.txt
```

3. Run the notebook:

```
jupyter notebook
```

---

## 🙌 Author

**Saugata Ghosh**

---

## ⭐ If you like this project, give it a star
