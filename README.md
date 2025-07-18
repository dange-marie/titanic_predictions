# 🛳️ Titanic - Machine Learning from Disaster

This project explores the classic Titanic dataset on Kaggle to predict passenger survival using machine learning techniques.  
It’s designed to reinforce the fundamentals of preprocessing, feature engineering, modeling, and validation.

## 🎯 Objective
Predict whether a passenger survived the Titanic disaster based on personal characteristics (class, sex, age, fare, etc.).

## 📊 Kaggle Score
- ✅ Public score: **0.76555**

## 🧠 Model Used
- Main model: **XGBoost Classifier**
- 5-fold cross-validation to avoid overfitting

## ⚙️ Engineered Features
- `Fare_log`: log transformation of the fare to reduce skew
- `Title`: extracted from the name (Mr, Miss, etc.)
- `Pont`: derived from cabin information
- One-hot encoding for `Embarked` categories
- Label encoding for `Sex`, `Ticket`, and others
- (Planned) `FamilySize` and `IsAlone` features

## 📂 Files
- `src/titanic_model.ipynb`: full notebook including preprocessing, feature engineering, training, and submission
- `output/submission.csv`: final submission file
- `README.md`: this file

## 🔧 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/titanic-kaggle.git
   cd titanic-kaggle
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Launch the notebook:

Use Jupyter Notebook or VS Code to open and run titanic_model.ipynb

📈 Next Steps
Add Optuna for hyperparameter tuning

Create FamilySize and IsAlone features

Try model stacking (XGBoost + Random Forest + Logistic Regression)

---

## 📦 Basic `requirements.txt` (recommended)
Create this file in your project root:

```txt
numpy
pandas
scikit-learn
xgboost
matplotlib
seaborn
jupyter
Then run:

bash
Copy
Edit
pip install -r requirements.txt
```

👤 Author
dange — Data scientist & computer science enthusiast

📬 [angelodsu22@gmail.com]
