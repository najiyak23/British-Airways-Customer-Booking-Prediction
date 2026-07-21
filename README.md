# ✈️ British Airways Customer Booking Prediction

A machine learning project that predicts whether a customer will complete a flight booking using historical booking data. The project includes data exploration, preprocessing, model development, evaluation, and feature importance analysis to provide actionable business insights.

---

## 📌 Project Overview

Airlines need to understand customer booking behavior to improve marketing strategies and increase booking conversions. This project builds a predictive model that estimates the likelihood of a customer completing a booking based on customer, flight, and booking information.

---

## 🎯 Objectives

- Explore and understand customer booking data.
- Prepare the dataset for machine learning.
- Train a classification model to predict booking completion.
- Evaluate model performance using multiple metrics.
- Identify the most influential features affecting booking decisions.

---

## 📂 Dataset

The dataset contains **50,000 customer booking records** with features including:

- Number of passengers
- Purchase lead time
- Length of stay
- Flight hour
- Flight duration
- Booking origin
- Sales channel
- Trip type
- Extra baggage preference
- Preferred seat selection
- In-flight meal preference

**Target Variable**

- `booking_complete`
  - `1` = Booking completed
  - `0` = Booking not completed

---

## 🔍 Exploratory Data Analysis

Performed the following analyses:

- Dataset exploration
- Missing value analysis
- Duplicate check
- Summary statistics
- Target class distribution
- Categorical feature identification

### Class Distribution

- **Completed Booking:** 14.96%
- **Not Completed:** 85.04%

The dataset is imbalanced, which was considered during model evaluation.

---

## ⚙️ Data Preprocessing

- One-Hot Encoding using `pd.get_dummies()`
- Feature and target separation
- Train-test split using stratified sampling

---

## 🤖 Machine Learning Model

**Algorithm Used**

- Random Forest Classifier

Random Forest was selected because it provides strong classification performance and enables feature importance analysis for model interpretation.

---

## 📊 Model Performance

| Metric | Score |
|---------|-------|
| Accuracy | **85.21%** |
| ROC-AUC | **0.792** |
| Precision | **0.53** |
| Recall | **0.10** |

---

## 📈 Top Important Features

The model identified the following variables as the strongest predictors of booking completion:

1. Purchase Lead
2. Length of Stay
3. Flight Hour
4. Booking Origin (Australia)
5. Flight Duration
6. Number of Passengers
7. Booking Origin (Malaysia)
8. Wants In-flight Meals
9. Wants Extra Baggage
10. Wants Preferred Seat

---

## 💡 Key Insights

- Purchase lead is the most influential factor in predicting booking completion.
- Trip characteristics such as length of stay, departure time, and flight duration significantly impact booking behavior.
- Customer preferences, including meal selection, baggage, and preferred seating, contribute to predicting completed bookings.
- Geographic booking origin also influences customer purchasing patterns.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 📁 Project Structure

```
British-Airways-Customer-Booking-Prediction/
│
├── data/
│   └── customer_booking.csv
│
├── notebooks/
│   └── customer_booking_prediction.ipynb
│
├── images/
│   └── feature_importance.png
│
├── presentation/
│   └── project_summary.pptx
│
└── README.md
```

---

## 🚀 Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Data Preprocessing
- Feature Engineering
- One-Hot Encoding
- Machine Learning Classification
- Random Forest
- Model Evaluation
- Cross Validation
- Feature Importance Analysis
- Business Insight Generation

---

## 📌 Results

The Random Forest model achieved strong overall predictive performance with an **Accuracy of 85.21%** and **ROC-AUC of 0.792**. Feature importance analysis revealed that booking lead time, trip characteristics, and customer service preferences are the primary drivers of booking completion, providing valuable insights for targeted marketing and customer engagement strategies.
