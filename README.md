# Ecommerce Customer Spending Analysis
## Linear Regression for Business Decision-Making

This repository contains a complete **end-to-end data analysis and machine learning project**
focused on understanding customer spending behavior in an ecommerce environment.

The company operates through both a **mobile application** and a **website**, and the primary
business question addressed in this project is:

> **Should the company focus more on improving its mobile app or its website?**

To answer this question, we apply **exploratory data analysis**, **statistical reasoning**, and
a **Linear Regression model** to extract actionable business insights.

---

## 📌 Project Motivation

Modern ecommerce companies collect vast amounts of behavioral data, yet many strategic
decisions are still made based on intuition rather than evidence.

This project demonstrates how **data-driven decision making** can be applied to:
- Understand customer engagement
- Quantify the impact of different platforms
- Support strategic investment decisions using machine learning

The dataset used in this project is synthetic and created solely for analytical purposes.

---

## 📊 Dataset Description

The dataset consists of **500 individual customers**, each represented by a single row.

### Features Included

| Feature | Description |
|------|------------|
| Avg. Session Length | Average duration of in-store style consultation sessions |
| Time on App | Average time spent using the mobile application |
| Time on Website | Average time spent using the website |
| Length of Membership | Duration of the customer's membership (in years) |
| Yearly Amount Spent | Total yearly spending (target variable) |

📷 **Dataset Preview**

![Dataset Overview](images/dataset_overview.png)

---

## 🧠 Methodology Overview

The project follows a structured data science workflow:

1. Data loading and inspection
2. Exploratory Data Analysis (EDA)
3. Feature selection and reasoning
4. Model training using Linear Regression
5. Model evaluation and diagnostics
6. Interpretation of coefficients
7. Business-oriented recommendations

Each step is fully documented in the Jupyter Notebook.

---

## 🔍 Exploratory Data Analysis (EDA)

EDA was performed to identify patterns, relationships, and potential predictors of
customer spending.

### Correlation Analysis

![Correlation Heatmap](images/correlation_heatmap.png)

Key observations:
- **Length of Membership** shows the strongest correlation with spending
- **Time on App** correlates more strongly with spending than **Time on Website**

---

### Feature Relationships

![Pairplot](images/pairplot.png)

From pairwise relationships:
- Spending increases noticeably with membership length
- App usage shows a clearer upward trend than website usage

---

## 🤖 Machine Learning Model

A **Linear Regression** model was selected due to:
- Interpretability
- Suitability for continuous target variables
- Clear coefficient-based explanations for business stakeholders

### Feature Matrix (X)
- Avg. Session Length
- Time on App
- Time on Website
- Length of Membership

### Target Variable (y)
- Yearly Amount Spent

---

## 📈 Model Evaluation

Model performance was evaluated using standard regression metrics:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

### Actual vs Predicted Values

![Actual vs Predicted](images/actual_vs_predicted.png)

Interpretation:
- Predictions align closely with actual values
- Most points lie near the ideal diagonal line
- Indicates strong predictive performance for strategic analysis

---

## 🧪 Residual Analysis

Residual analysis was conducted to validate model assumptions.

### Residual Distribution

![Residual Distribution](images/residual_distribution.png)

- Residuals are centered around zero
- Distribution is approximately normal

### Residuals vs Predictions

![Residuals vs Predictions](images/residuals_vs_predictions.png)

- No clear pattern observed
- Suggests absence of systematic bias in predictions

---

## 📊 Model Interpretation

The model coefficients provide insights into how each feature impacts spending.

Key insights:
- **Length of Membership** is the most influential factor
- **Time on App** has a stronger positive effect than **Time on Website**
- Website engagement appears to have a weaker marginal impact

These findings are particularly valuable for strategic investment decisions.

---

## 💡 Business Recommendation

Based on the analysis and model interpretation:

### ✅ Final Recommendation

The company should prioritize **enhancing the mobile app experience**, as customer
engagement on the app is more strongly associated with increased yearly spending
compared to website usage.

Additionally, strategies that **increase customer retention and membership duration**
are likely to yield the highest returns.

---

## ⚠️ Model Limitations

While the model provides valuable insights, it has limitations:

- Assumes linear relationships between variables
- Does not include external influences such as promotions or seasonality
- Intended for strategic guidance rather than individual-level predictions

Future work could involve:
- Regularization techniques (Ridge, Lasso)
- Non-linear models
- Time-series analysis

---

## 🛠️ Technologies Used

- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn
- Jupyter Notebook

---

## ▶️ How to Run the Project

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```bash
3. Launch the notebook: 
    ```bash
jupyter notebook notebooks/01_ecommerce_linear_regression.ipynb
    ```bash

## 📁 Project Structure

ecommerce-customer-spending-analysis/
│
├── data/
│   └── EcommerceCustomers.csv
│
├── notebooks/
│   └── 01_ecommerce_linear_regression.ipynb
│
├── images/
│   └── *.png
│
├── README.md
├── requirements.txt
└── .gitignore

## 👤 Author

This project was created as a portfolio-level data science project to demonstrate
practical application of machine learning for business decision-making.