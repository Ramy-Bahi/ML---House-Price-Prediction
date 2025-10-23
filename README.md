# ML-House-Price-Prediction
Machine Learning project comparing Linear and Polynomial Regression on housing data.

---

# 🏠 House Prices Prediction — Linear & Polynomial Regression

This project explores **Machine Learning regression techniques** on the [House Prices: Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) dataset from Kaggle.  
It’s part of my journey to fully master **Machine Learning** before moving into **Deep Learning**.

---

## 📘 Project Overview

The goal is to predict the **Sale Price** of residential homes based on multiple numerical and categorical features.

This project is divided into two separate notebooks:

| Notebook | Description |
|-----------|--------------|
| 📓 `linear_regression.ipynb` | Builds a clean linear regression pipeline with full preprocessing, encoding, scaling, and evaluation. |
| 📓 `polynomial_regression.ipynb` | Extends the linear model using polynomial features (degree = 2) to explore non-linear relationships. |

---

## ⚙️ Technologies Used

- **Python 3.x**
- **NumPy**, **Pandas** → data manipulation  
- **Matplotlib**, **Seaborn** → visualization  
- **Scikit-Learn** → regression, preprocessing, evaluation  
- **SciPy** → skewness correction  

---

## 🧩 Data Preprocessing Pipeline

1. Handle missing values  
2. Encode categorical variables (One-Hot Encoding)  
3. Map ordinal quality features (`Ex`, `Gd`, `TA`, etc.)  
4. Correct skewed numeric features using `log1p`  
5. Scale features using `StandardScaler`  
6. Train & evaluate regression models  

---

## 📊 Model Results

| Model | R² | Cross-Validation | RMSE | MAE |
|-------|----|------------------|------|-----|
| **Linear Regression** | 0.766 | **0.72** | 42,391 | **22,173** |
| **Polynomial Regression (deg=2)** | **0.786** | 0.67 | **40,523** | 28,044 |

### 🧠 Insights
- Polynomial Regression fit training data slightly better  
- However, Linear Regression generalized better on unseen data  
- Skew correction & feature engineering improved both models significantly  

---

## 🚀 Next Steps

- Add **Decision Tree**, **Random Forest**, and **XGBoost** regressors  
- Try **log(SalePrice)** target transformation  
- Transition to **Deep Learning** (Neural Networks for regression)

---

## 🧾 Repository Structure

House-Prices-Regression/
│
├── data/
│ ├── train.csv
│ ├── test.csv
│
├── notebooks/
│ ├── linear_regression.ipynb
│ └── polynomial_regression.ipynb
│
├── requirements.txt
├── README.md
└── .gitignore

---

## 🧩 How to Run

```bash
git clone https://github.com/<yourusername>/House-Prices-Regression.git
cd House-Prices-Regression
pip install -r requirements.txt
jupyter notebook notebooks/linear_polynomial_regression.ipynb
```

---

📊 Dataset

Available on Kaggle: https://www.kaggle.com/c/house-prices-advanced-regression-techniques

---

👨‍💻 Author

**Rami Bahi**

🎓 Master’s Student in Artificial Intelligence

💻 Passionate about Machine Learning, Deep Learning & Web Development

---

⭐ If you like this project

Give it a star ⭐ on GitHub to support my work and journey!
