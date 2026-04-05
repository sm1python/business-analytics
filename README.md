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
