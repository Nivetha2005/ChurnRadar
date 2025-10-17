# ChurnRadar

## Project Overview

ChurnRadar is an interactive dashboard and analysis project designed to study customer churn in a retail bank. It combines Python-based data exploration and machine learning with Power BI visualizations to provide insights into customer behavior, financial patterns, and churn prediction.

## Folder Structure

```
ChurnRadar/
│
├── Data/
│   └── Customer-Churn-Records.csv          # Raw dataset
│
├── Notebooks/
│   └── churnRadar.ipynb                     # Jupyter notebook for EDA, preprocessing, and modeling
│
├── Models/
│   ├── model.pkl                            # Trained ML model for churn prediction
│   └── scaler.pkl                           # StandardScaler object used for preprocessing
│
├── PowerBI/
│   ├── ChurnRadar.pbix                      # Power BI dashboard file
│   └── ChurnRadar.pdf                       # Exported PDF of the dashboard
│
└── README.md                                # Project overview and instructions
```

## Features

* **Customer Overview:** Total customers, churn rate, active members, card holders.
* **Univariate Analysis:** Histograms, boxplots, and distribution charts for numerical features; pie charts for categorical features.
* **Bivariate Analysis:** Correlation plots, churn patterns by demographic and financial features.
* **Predictive Insights:** ML model predicting customer churn using features like Age, CreditScore, Balance, etc.
* **Interactive Dashboard:** Power BI dashboard with slicers for Geography, Gender, Card Type, and Membership status.

## How to Use

1. **Power BI Dashboard:**

   * Open `PowerBI/ChurnRadar.pbix` in Power BI Desktop.
   * Load the dataset from `Data/Customer-Churn-Records.csv`.
   * Explore visuals and use slicers to filter data interactively.

2. **Python Notebook:**

   * Open `Notebooks/churnRadar.ipynb` to view preprocessing, EDA, and model training steps.
   * The notebook uses `Models/model.pkl` and `Models/scaler.pkl` for predictions.

## Requirements

* Python 3.x
* Libraries: pandas, numpy, matplotlib, seaborn, scipy, scikit-learn, xgboost, feature-engine, tabulate, pickle
* Power BI Desktop

## Notes

* Ensure `Customer-Churn-Records.csv` is in the Data folder before running the notebook or loading the dashboard.
* Model and scaler are pre-trained; you can retrain using the notebook if needed.
