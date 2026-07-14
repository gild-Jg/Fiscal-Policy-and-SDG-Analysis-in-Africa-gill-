# 📊 Fiscal Policy and SDG Analysis in Africa
![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy)
![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?logo=scikitlearn)
![XGBoost](https://img.shields.io/badge/XGBoost-ML-green)
![Power%20BI](https://img.shields.io/badge/Power_BI-F2C811?logo=powerbi)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?logo=kaggle)
![GitHub](https://img.shields.io/badge/GitHub-Portfolio-black?logo=github)
![License](https://img.shields.io/badge/License-MIT-green)
## Leveraging Data Science and Machine Learning to Evaluate Fiscal Policy and Sustainable Development Across Africa

## 📖 Project Overview:
This project investigates the relationship between fiscal policy and economic growth across selected African countries using macroeconomic and government finance indicators.The analysis combines Exploratory Data Analysis (EDA), feature engineering, statistical analysis, and machine learning to identify the fiscal indicators that are most strongly associated with GDP Growth Rate.The study aligns fiscal indicators with selected Sustainable Development Goals (SDGs) to demonstrate how data-driven approaches can support evidence-based policymaking.

## 🎯 Objectives:
  - Analyze fiscal and macroeconomic indicators across selected African countries.
  - Investigate relationships between fiscal variables and GDP Growth Rate.
  - Map fiscal indicators to selected Sustainable Development Goals (SDGs).
  - Build predictive machine learning models for GDP Growth Rate.
  - Compare model performance and identify the most suitable algorithm.
  - Generate policy insights from the analytical findings.

## 📂 Dataset
The project combines data from multiple international sources including:
  - International Monetary Fund (IMF)
  - World Bank Open Data
  - World Bank Exchange Rate API

## Countries included:
  - Egypt
  - Kenya
  - Nigeria
  - South Africa
The final analytical dataset contains fiscal, macroeconomic, and trade indicators spanning multiple years.

## 🛠 Technologies:
  - Python 
  - Pandas
  - NumPy
  - Matplotlib
  - Seaborn
  - Scikit-learn
  - XGBoost
  - Kaggle Notebooks
  - GitHub
  - Power BI
---
## 🔬 Methodology
This project followed the **CRISP-DM (Cross-Industry Standard Process for Data Mining)** framework, providing a structured approach from data collection to model evaluation.

### 1. Data Collection
  - Retrieved fiscal and macroeconomic data from the International Monetary Fund (IMF).
  - Collected exchange rate data using the World Bank API.
  - Integrated datasets into a unified analytical dataset.

### 2. Data Cleaning & Preparation
  - Standardized indicator names and measurement units.
  - Removed duplicates and inconsistent records.
  - Handled missing values and merged datasets.
  - Created checkpoint datasets using Parquet for reproducibility.

### 3. Exploratory Data Analysis (EDA)
  - Analyzed trends and distributions of fiscal indicators.
  - Examined relationships using correlation analysis and scatter plots.
  - Conducted SDG-focused analyses to assess fiscal performance across selected Sustainable Development Goals.

### 4. Feature Engineering
  - Selected features based on data completeness, correlation analysis, and mutual information.
  - Constructed the final modelling dataset using the most informative fiscal indicators.

### 5. Data Preprocessing
  - Imputed missing values using mean imputation.
  - Selected countries with sufficient data coverage.
  - Split the data into training and testing sets.
  - Applied feature scaling where appropriate for model requirements.

### 6. Machine Learning
The following regression models were developed and compared:
  - Linear Regression
  - Decision Tree Regressor
  - Random Forest Regressor
  - XGBoost Regressor

### 7. Model Evaluation
Models were evaluated using:
  - Coefficient of Determination (R²)
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)
  - Feature Importance Analysis
  - Hyperparameter Tuning (GridSearchCV)
  - Cross Validation
---
## 📈 Project Workflow

```
Raw IMF & World Bank Data
           │
           ▼
     Data Cleaning
           │
           ▼
   Data Integration
           │
           ▼
 Exploratory Data Analysis
           │
           ▼
 Feature Engineering
           │
           ▼
 Data Preprocessing
           │
           ▼
 Machine Learning
           │
           ▼
 Model Evaluation
           │
           ▼
 Interpretation & Policy Insights
```

---

## 🤖 Machine Learning Models

Four supervised machine learning regression models were developed and evaluated to predict **GDP Growth Rate** from selected fiscal and macroeconomic indicators.

| Model | Purpose |
|--------|---------|
| Linear Regression | Baseline model to evaluate linear relationships between fiscal indicators and GDP Growth Rate. |
| Decision Tree Regressor | Captures non-linear relationships and provides interpretable decision rules. |
| Random Forest Regressor | Ensemble learning model used to improve predictive performance and reduce overfitting. |
| XGBoost Regressor | Gradient boosting model designed to capture complex relationships and improve prediction accuracy. |

Following model comparison and hyperparameter tuning, the **Decision Tree Regressor** was selected as the final model due to its superior balance between predictive performance and generalization.
---

## 📊 Results And Key Findings

### Exploratory Data Analysis (EDA)

- Identified strong positive relationships between government revenue and expenditure.
- Correlation analysis revealed significant associations among fiscal and macroeconomic indicators.
- SDG-focused analysis demonstrated varying fiscal performance across the selected African countries.

### Machine Learning

- Seven key predictors were selected through feature engineering:
  - Government Debt
  - Revenue
  - Exports
  - Imports
  - Nominal GDP
  - Real GDP
  - Year

- **Target Variable:** GDP Growth Rate

### Best Performing Model

- **Model:** Decision Tree Regressor
- **Test R² Score:** **0.279**
- **Test MAE:** **0.0255**

### Key Findings

- Government Debt emerged as the most influential predictor of GDP Growth Rate.
- Real GDP, Nominal GDP, and Exports also contributed significantly to model predictions.
- Hyperparameter tuning improved the Decision Tree's predictive performance.
- Cross-validation indicated limited generalizability due to the small sample size, panel structure of the data, and incomplete indicator coverage.

---

## 📁 Repository Structure

```
Fiscal-Policy-and-SDG-Analysis-in-Africa/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   └── Fiscal_Policy_SDG_Analysis.ipynb
│
├── dashboard/
│   └── Fiscal_Dashboard.pbix
│
├── presentation/
│   └── Final_Presentation.pptx
│
├── images/
│
├── models/
│
├── reports/
│
├── README.md
├── requirements.txt
└── LICENSE
```
The repository is organized to separate raw data, processed datasets, notebooks, dashboards, presentations, reports, and supporting resources, making the project easy to navigate and reproduce.

---

## 📊 Interactive Dashboard

A Power BI dashboard was developed to complement the notebook by providing an interactive visualization of fiscal and macroeconomic indicators.

The dashboard enables users to:

- Compare fiscal performance across countries.
- Explore trends in GDP Growth Rate.
- Analyze government revenue, expenditure, debt, imports, and exports.
- Filter results by country and year.
- Support data-driven fiscal policy analysis.

> **Dashboard Location:** `/dashboard/Fiscal_Dashboard.pbix`
---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/gild-jg/Fiscal-Policy-and-SDG-Analysis-in-Africa.git
```

Navigate into the project directory:

```bash
cd Fiscal-Policy-and-SDG-Analysis-in-Africa
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```
notebooks/Fiscal_Policy_SDG_Analysis.ipynb
```

to reproduce the analysis.
---

## 🚀 Future Work

Potential extensions of this project include:

- Expanding the analysis to include additional African countries.
- Incorporating longer historical time series.
- Integrating additional macroeconomic and governance indicators.
- Exploring advanced machine learning and deep learning models.
- Developing time-series forecasting models for GDP Growth.
- Deploying the project as an interactive web application.
- Enhancing the Power BI dashboard with real-time data integration.

---

## 🚀 Future Work

Potential extensions of this project include:

- Expanding the analysis to include additional African countries.
- Incorporating longer historical time series.
- Integrating additional macroeconomic and governance indicators.
- Exploring advanced machine learning and deep learning models.
- Developing time-series forecasting models for GDP Growth.
- Deploying the project as an interactive web application.
- Enhancing the Power BI dashboard with real-time data integration.

  ---

## 👨‍💻 Author

**Gill Finidi Omondi**

Bachelor of Quantity Surveying (Technical University of Kenya)

Data Science | Quantity Surveyor  | Construction Cost Management Enthusiast

### Connect with Me

- GitHub: https://github.com/gild-jg
- LinkedIn: *(Gill Finidi)*
- Kaggle: *(djg001)*

---

## 🙏 Acknowledgements

This project was developed using publicly available data and open-source tools.

Special thanks to:

- International Monetary Fund (IMF) for fiscal and macroeconomic datasets.
- World Bank Open Data for macroeconomic indicators and exchange rate data.
- 10Alytics for organizing the hackathon and providing the opportunity to apply data science to real-world public finance challenges.
- The open-source Python community for the tools and libraries that made this analysis possible.






