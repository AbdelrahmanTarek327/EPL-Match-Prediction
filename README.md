# EPL-Match-Prediction
Predicting English Premier League match outcomes using machine learning

# 🏆 EPL Match Outcome Prediction

Predicting English Premier League (EPL) match outcomes — Home Win, Draw, or Away Win — using machine learning models trained on 2000–2024 match data.

## 📊 Dataset

- Source: [Kaggle EPL Dataset](https://www.kaggle.com/datasets/stephenyulinchen/epl-2425-data/data)
- Features: Goals, Cards, Shots, Fouls, etc.
- Target: Match result (FTR)

## 🛠️ Tools & Libraries

- Python, Pandas, NumPy
- Scikit-learn, XGBoost, Joblib
- Matplotlib, Seaborn

## 🧹 Preprocessing

- Removed 1 row with missing values
- Converted `Date` to datetime
- Dropped `Referee` column due to high cardinality

## 📈 Exploratory Analysis

- Class distribution
- Correlation heatmap



## 🤖 Models Used

- Logistic Regression
- K-Nearest Neighbors
- Decision Tree
- Random Forest
- XGBoost

## 🧠 Best Model

- **XGBoost**
- Accuracy: 100%
- Model saved as `epl_model.pkl`

## 🧪 Deployment

Model saved using `joblib`. Can be deployed using Flask or Streamlit.

```python
import joblib
model = joblib.load('epl_model.pkl')
