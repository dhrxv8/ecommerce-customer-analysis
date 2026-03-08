# 📊 Ecommerce App vs. Website — Sales Impact Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-red?logo=scikit-learn)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

## 📌 Overview

This project applies **Linear Regression** to analyze customer behavior data for an Ecommerce company to determine whether they should invest more in their **mobile app** or **website** to boost yearly sales. The analysis covers exploratory data visualization, model training, and evaluation using Python.

---

## 🎯 Objective

To identify which platform — mobile app or website — has a greater influence on the **Yearly Amount Spent** by customers, and provide data-driven recommendations for business strategy.

---

## 🗂️ Dataset

- **File:** `Ecommerce Customers` (CSV)
- **Records:** 500 customer entries (no missing values)
- **Features used for modeling:**

| Feature | Description |
|---|---|
| `Avg. Session Length` | Average in-store style advice session length |
| `Time on App` | Time spent on the mobile app (minutes) |
| `Time on Website` | Time spent on the website (minutes) |
| `Length of Membership` | Number of years as a member |

- **Target Variable:** `Yearly Amount Spent`

---

## 🔍 Exploratory Data Analysis

- Joint plots comparing `Time on App` and `Time on Website` against `Yearly Amount Spent`
- Hex bin plot for `Time on App` vs `Length of Membership`
- Pair plots across all numerical features to identify correlations
- Linear model plot showing `Length of Membership` vs `Yearly Amount Spent`

---

## 🤖 Model

- **Algorithm:** Linear Regression (`sklearn.linear_model.LinearRegression`)
- **Train/Test Split:** 70% train / 30% test (`random_state=101`)

### Model Coefficients

| Feature | Coefficient |
|---|---|
| Length of Membership | **61.28** |
| Time on App | **38.59** |
| Avg. Session Length | **25.98** |
| Time on Website | **0.19** |

### Model Evaluation Metrics

| Metric | Value |
|---|---|
| MAE | 7.23 |
| MSE | 79.81 |
| RMSE | 8.93 |

Residuals are approximately normally distributed, confirming a good model fit.

---

## 💡 Key Insights

- **Length of Membership** is the strongest predictor of yearly spending (coefficient: 61.28), meaning long-term customer retention has the biggest impact on revenue.
- **Time on App** (coeff: 38.59) significantly outperforms **Time on Website** (coeff: 0.19), suggesting the mobile app is a far more effective sales channel.
- **Recommendation:** The company should prioritize improving the **mobile app experience** and focus on **customer retention strategies** to maximize yearly revenue.

---

## 🛠️ Technologies Used

| Tool | Purpose |
|---|---|
| Python 3 | Core programming language |
| Pandas | Data manipulation & exploration |
| NumPy | Numerical computations |
| Matplotlib | Static visualizations |
| Seaborn | Statistical visualizations |
| scikit-learn | Linear regression model & evaluation |
| Jupyter Notebook | Interactive analysis environment |

---

## 📁 Project Structure

```
Linear_regression/
│
├── Linear Regression Project.ipynb   # Main analysis notebook
├── Ecommerce Customers                # Dataset (CSV)
└── README.md                          # Project documentation
```

---

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/dhrxv8/Linear_regression.git
cd Linear_regression

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Launch the notebook
jupyter notebook "Linear Regression Project.ipynb"
```

---

## 📬 Contact

**Dhruv**
🔗 [GitHub Profile](https://github.com/dhrxv8)