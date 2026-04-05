# business-analytics
## End-to-End Business Analytics & Sales Prediction Pipeline

### Project Overview
This project addresses a real-world retail business problem: **Analyzing sales trends and forecasting future revenue.** By leveraging historical transaction data, customer demographics, and product information, this pipeline aims to provide actionable insights for inventory management and financial planning.

The project follows a comprehensive machine learning workflow, including:
* Data Pre-processing & Cleaning
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Predictive Modeling (Ensemble Stacking & AutoGluon)
* Model Explainability (SHAP)
* Performance Evaluation

### Repository Structure
Following professional standards, the repository is organized as follows:

```text
├── data/                   # Dataset directory
│   ├── products.csv        # Product categories and costs
│   ├── transactions.csv    # Historical sales records
│   ├── customers.csv       # Customer demographic data
│   ├── employees.csv       # Staff information
│   ├── stores.csv          # Store locations and employee counts
│   └── discounts.csv       # Seasonal promotion data
├── notebooks/              # Analysis and modeling
│   └── Final Project-BA.ipynb
└── README.md               # Project documentation
```

### Dataset Description
The analysis utilizes six interconnected datasets:

* **Transactions**: Core sales data including invoice IDs, quantities, and totals.
* **Products**: Details on categories (e.g., Feminine, Men), sizes, and production costs.
* **Customers**: Demographic info including City, Country, Gender, and Job Titles.
* **Stores**: Geographic data and store-level metrics.
* **Employees**: Organizational structure and staff positions.
* **Discounts**: Historical discount rates for specific periods and categories.

### Methodology

#### 1. Exploratory Data Analysis (EDA)
Comprehensive cleaning and visualization were performed to identify seasonal trends, top-performing product categories, and customer purchasing patterns.

#### 2. Predictive Modeling
To achieve high accuracy, we implemented a **Stacked Regressor** model:
* **Base Learners**: XGBoost, CatBoost, and LightGBM.
* **Meta-Learner**: Ridge Regression (Final Estimator).
* **Alternative**: Automated machine learning via **AutoGluon TabularPredictor** for hyperparameter tuning and model selection.

#### 3. Explainability & Confidence
* **SHAP Analysis**: Used to interpret model predictions and identify which features (like price or category) most significantly impact sales.
* **Uncertainty Estimation**: 95% Confidence Intervals were calculated for all forecasts to provide a range of probable outcomes rather than just a single point estimate.

### Installation
To run the analysis locally, ensure you have the following libraries installed:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost catboost lightgbm autogluon shap
```
__python==1.13.1__
