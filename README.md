# Ecommerce Customer Spending Analysis

<img width="2752" height="1536" alt="Gemini_Generated_Image_xjngw2xjngw2xjng" src="https://github.com/user-attachments/assets/9ca19e21-d7c9-42ae-bd21-cd725f10f73b" />

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

<img width="736" height="273" alt="Ekran Resmi 2026-01-21 14 57 25" src="https://github.com/user-attachments/assets/ddf42f15-4f63-45a1-a07e-8321e1dc9a0b" />

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

<img width="769" height="667" alt="Unknown-1" src="https://github.com/user-attachments/assets/b9592bf5-452e-4946-b452-0c6bc541c492" />


Key observations:
- **Length of Membership** shows the strongest correlation with spending
- **Time on App** correlates more strongly with spending than **Time on Website**

---

### Feature Relationships

<img width="1228" height="1228" alt="Unknown" src="https://github.com/user-attachments/assets/204c162b-8b14-4e3d-9848-ea0ff3b451dd" />

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

<img width="784" height="584" alt="Unknown-2" src="https://github.com/user-attachments/assets/075df3f8-acd6-4982-bf47-a6b583bc0d63" />

Interpretation:
- Predictions align closely with actual values
- Most points lie near the ideal diagonal line
- Indicates strong predictive performance for strategic analysis

---

## 🧪 Residual Analysis

Residual analysis was conducted to validate model assumptions.

### Residual Distribution

<img width="613" height="473" alt="Unknown-3" src="https://github.com/user-attachments/assets/2f587394-7613-4850-85fd-6b90d22e231d" />

- Residuals are centered around zero
- Distribution is approximately normal

### Residuals vs Predictions

<img width="622" height="473" alt="Unknown-4" src="https://github.com/user-attachments/assets/aa191659-aa63-4153-803e-fda5dd281622" />

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

customer-spending-prediction-ml/
│
├── data/
│   └── EcommerceCustomers.csv
│       # Raw dataset containing customer behavior and yearly spending information
│
├── images/
│   ├── ActualVsPredictedSpending.png
│   │   # Seaborn visualization comparing actual vs predicted spending values
│   ├── CorrelationMatrix.png
│   │   # Correlation heatmap of numerical features
│   ├── DatasetStructure.png
│   │   # Overview of dataset structure and columns
│   ├── ExploratoryDataAnalysis.png
│   │   # Key EDA visualizations
│   ├── ResidualDistribution.png
│   │   # Distribution of residuals from the regression model
│   └── ResidualsVsPredictedValues.png
│       # Residuals plotted against predicted values
│
├── notebooks/
│   └── 01_ecommerce_linear_regression.ipynb
│       # Main Jupyter Notebook containing EDA, modeling, evaluation, and insights
│
├── README.md
│   # Comprehensive project documentation and results
│
├── requirements.txt
│   # Python dependencies required to run the project
│
└── .gitignore
    # Files and folders excluded from version control


## 👤 Author

This project was created as a portfolio-level data science project to demonstrate
practical application of machine learning for business decision-making.
