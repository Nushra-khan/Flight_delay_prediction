# ✈️ Flight Delay Prediction using Machine Learning

## 🔍 Overview

Flight delays are a common inconvenience in the airline industry, affecting passenger satisfaction and airline profitability. This project aims to build a machine learning model that predicts whether a flight will be delayed by more than 60 minutes, using features like airline, departure time, day of the week, and more.

---

## 📁 Dataset

- **Source**: [DeepCharts YouTube Channel](https://www.youtube.com/@DeepCharts)
- **File Used**: `Flight_delay.csv`
- **Selected Features**:
  - `DayOfWeek`, `Date`, `DepTime`, `Airline`, `Origin`, `Dest`, `CarrierDelay`

---

## 🧠 Modeling

Multiple classification algorithms were implemented and compared:

- ✅ **Logistic Regression**
- 🌲 **Decision Tree Classifier**
- 🌳 **Random Forest Classifier**
- ⚡ **XGBoost Classifier**

### Key Techniques Used:
- Train-test split (80-20)
- Hyperparameter tuning with `GridSearchCV`
- Class imbalance handled using `class_weight='balanced'`
- One-hot encoding for categorical variables
- Target variable: 1 if `CarrierDelay > 60`, else 0

---

## 📊 Evaluation

- Metrics used:
  - Accuracy
  - Precision, Recall, F1-Score
  - Confusion Matrix
  - ROC Curve and AUC Score

Each model was evaluated and compared to select the best-performing one.

---

## 🔧 Technologies Used

- Python, Jupyter Notebook
- pandas, numpy, seaborn, matplotlib
- scikit-learn, xgboost

---

## 🚀 How to Run

1. Clone the repository:
```bash
git clone https://github.com/yourusername/flight-delay-prediction.git
cd flight-delay-prediction
