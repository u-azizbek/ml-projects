# ML Projects

A curated collection of machine learning, data analysis, and data engineering projects covering supervised learning algorithms, time series forecasting, natural language processing, exploratory data analysis, web scraping, and SQL-based data exploration.

---

## Table of Contents

- [Projects Overview](#projects-overview)
- [Tech Stack](#tech-stack)
- [Project Details](#project-details)
- [Getting Started](#getting-started)
- [Repository Structure](#repository-structure)

---

## Projects Overview

| # | Project | Category | Algorithm / Technique |
|---|---------|----------|-----------------------|
| 1 | [Linear Regression](#1-linear-regression) | Supervised Learning | Simple Linear Regression |
| 2 | [Multiple Regression](#2-multiple-regression) | Supervised Learning | Multiple Linear Regression |
| 3 | [Polynomial Regression](#3-polynomial-regression) | Supervised Learning | Polynomial Regression |
| 4 | [Decision Tree Regression](#4-decision-tree-regression) | Supervised Learning | Decision Tree Regressor |
| 5 | [Support Vector Regression](#5-support-vector-regression-svr) | Supervised Learning | SVR with Feature Scaling |
| 6 | [PJME Time Series Analysis](#6-pjme-time-series-analysis) | Time Series | XGBoost + Feature Engineering |
| 7 | [Time Series Forecasting](#7-time-series-forecasting) | Time Series | XGBoost + Cross-Validation |
| 8 | [Spam Classifier](#8-spam-classifier) | NLP | Naive Bayes |
| 9 | [Optimized Spam](#9-optimized-spam--ensembles) | NLP | Ensemble Methods |
| 10 | [EDA Analysis](#10-exploratory-data-analysis) | Data Analysis | EDA on Unicorn Companies |
| 11 | [Data Preprocessing](#11-data-preprocessing) | Data Engineering | Preprocessing Pipeline |
| 12 | [Netflix Movies Investigation](#12-netflix-movies--guest-stars-investigation) | Data Analysis | Pandas + Visualization |
| 13 | [Web Scraping](#13-amazon-web-scraper) | Data Engineering | BeautifulSoup + Requests |
| 14 | [SQL Projects](#14-sql--covid-19-data-exploration) | Data Engineering | SQL Data Exploration |

---

## Tech Stack

**Languages:** Python 3, SQL

**Libraries & Frameworks:**

| Category | Libraries |
|----------|-----------|
| Data Manipulation | `pandas`, `numpy` |
| Machine Learning | `scikit-learn`, `xgboost` |
| Visualization | `matplotlib`, `seaborn` |
| NLP | `sklearn.feature_extraction`, `nltk` |
| Web Scraping | `beautifulsoup4`, `requests` |
| Notebook Environment | `Jupyter Notebook / JupyterLab` |

---

## Project Details

### 1. Linear Regression
**Folder:** `Linear Regression/`  
**Dataset:** `Salary_Data.csv`

Predicts employee salary based on years of experience using simple linear regression. Includes train/test split, model fitting, and scatter plot visualizations comparing training vs. test set predictions.

**Key concepts:** `LinearRegression`, train/test split, regression visualization.

---

### 2. Multiple Regression
**Folder:** `Multiple Regression/`  
**Dataset:** `50_Startups.csv`

Predicts startup profit using multiple input features including R&D spend, administration cost, marketing spend, and geographic state. Implements one-hot encoding for categorical variables.

**Key concepts:** `LinearRegression`, `ColumnTransformer`, `OneHotEncoder`, multiple features.

---

### 3. Polynomial Regression
**Folder:** `Polynomial Regression/`  
**Dataset:** `Position_Salaries.csv`

Compares linear vs. polynomial regression on a position salary dataset to demonstrate underfitting vs. better fit with higher-degree polynomial features. Also includes a Euro 2012 football statistics analysis notebook.

**Key concepts:** `PolynomialFeatures`, `LinearRegression`, model comparison.

---

### 4. Decision Tree Regression
**Folder:** `Decision Tree/`  
**Dataset:** `Position_Salaries.csv`

Applies a decision tree regressor to predict salaries based on job position level, demonstrating non-linear, step-wise prediction behaviour characteristic of tree-based models.

**Key concepts:** `DecisionTreeRegressor`, non-linear regression, tree depth.

---

### 5. Support Vector Regression (SVR)
**Folder:** `SVR/`  
**Dataset:** `Position_Salaries.csv`

Implements SVR with feature scaling to predict position-based salaries. Highlights the importance of normalizing both features and target variables before fitting an SVR model.

**Key concepts:** `SVR`, `StandardScaler`, feature scaling, kernel methods.

---

### 6. PJME Time Series Analysis
**File:** `pjme_time_series_analysis.ipynb`  
**Dataset:** `PJME_hourly.csv`

Analyzes hourly energy consumption data from the PJM Interconnection (PJME region). Builds temporal features (hour, day of week, month, quarter, year) and trains an XGBoost model to forecast energy usage in megawatts.

**Key concepts:** `XGBRegressor`, time-based feature engineering, train/test split by date, `mean_squared_error`.

---

### 7. Time Series Forecasting
**File:** `time_series_forecasting.ipynb`  
**Dataset:** `PJME_hourly.csv`

An extended and optimized version of the PJME analysis. Adds outlier detection and removal, time series cross-validation using `TimeSeriesSplit`, lag features, and rolling window statistics for improved model robustness.

**Key concepts:** `TimeSeriesSplit`, outlier removal, lag features, rolling mean/std, `XGBRegressor`.

---

### 8. Spam Classifier
**Folder:** `Spam Classifier/`  
**Dataset:** `SMSSpamCollection`

Builds an SMS spam detection pipeline from scratch using Naive Bayes. Walks through tokenization, bag-of-words vectorization, Laplace smoothing, and Bayesian inference before using scikit-learn's `MultinomialNB` for a clean implementation.

**Key concepts:** `CountVectorizer`, `MultinomialNB`, Bayesian inference, precision, recall, F1-score.

---

### 9. Optimized Spam & Ensembles
**Folder:** `Optimized Spam/`  
**Dataset:** `SMSSpamCollection`

An optimized take on spam classification using ensemble methods alongside Naive Bayes. Evaluates models with accuracy, precision, recall, and F1 metrics and compares performance across classifiers.

**Key concepts:** Ensemble methods, `MultinomialNB`, `CountVectorizer`, model evaluation metrics.

---

### 10. Exploratory Data Analysis
**Folder:** `eda_analysis/`  
**Dataset:** `Unicorn_Companies.csv`

Performs exploratory data analysis on global unicorn companies (startups valued at $1B+). Investigates funding distributions, industry breakdowns, and geographic trends using pandas and visualization libraries.

**Key concepts:** EDA, data profiling, `pandas`, `matplotlib`, `seaborn`.

---

### 11. Data Preprocessing
**Folder:** `Data Preprocessing/`  
**Dataset:** `Data.csv`

A reusable preprocessing template demonstrating the full standard pipeline: importing data, handling missing values, encoding categorical variables, feature scaling, and splitting into training and test sets.

**Key concepts:** Missing value imputation, `SimpleImputer`, `LabelEncoder`, `StandardScaler`, train/test split.

---

### 12. Netflix Movies & Guest Stars Investigation
**Folder:** `Investigating Netflix Movies and Guest Stars in The Office/`  
**Datasets:** `netflix_data.csv`, `color_data.csv`

Investigates whether the average duration of Netflix movies has been declining over the years. Analyzes movie and TV show data and visualizes trends, including a fun look at guest star appearances in *The Office*.

**Key concepts:** Dictionary to DataFrame, filtering, `matplotlib` line and scatter plots, color-coded visualizations.

---

### 13. Amazon Web Scraper
**Folder:** `Web Scraping/`

Scrapes product title and price data from an Amazon product page using `BeautifulSoup` and `requests`. Stores data to a CSV file and includes an automated price-check loop that sends an email alert when the price drops below a defined threshold.

**Key concepts:** `BeautifulSoup`, `requests`, HTML parsing, `smtplib`, automated price monitoring.

---

### 14. SQL – COVID-19 Data Exploration
**Folder:** `SQL Projects/`

Explores global COVID-19 data using SQL Server. Covers total cases vs. deaths, infection rates relative to population, vaccination rollout analysis, rolling sums with window functions, and CTEs/temp tables for staged queries.

**Key concepts:** `JOIN`, `GROUP BY`, window functions (`OVER`, `PARTITION BY`), CTEs, temp tables, aggregate calculations.

---

## Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook or JupyterLab

### Installation

1. Clone or download this repository:
   ```bash
   git clone <repository-url>
   cd ml-projects
   ```

2. Install the required Python packages:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn xgboost beautifulsoup4 requests
   ```

3. Launch Jupyter:
   ```bash
   jupyter notebook
   ```

4. Navigate to any project folder and open the `.ipynb` notebook.

---

## Repository Structure

```
ml-projects/
├── Data Preprocessing/
│   ├── data_preprocessing.ipynb
│   └── Data.csv
├── Decision Tree/
│   ├── decision_tree_regression.ipynb
│   └── Position_Salaries.csv
├── eda_analysis/
│   ├── exploratory_data_analysis.ipynb
│   └── Unicorn_Companies.csv
├── Investigating Netflix Movies and Guest Stars in The Office/
│   ├── notebook.ipynb
│   └── datasets/
│       ├── netflix_data.csv
│       └── color_data.csv
├── Linear Regression/
│   ├── Linear Regression.ipynb
│   └── Salary_Data.csv
├── Multiple Regression/
│   ├── multiple_linear_regression.ipynb
│   └── 50_Startups.csv
├── Optimized Spam/
│   └── Spam_&_Ensembles_Solution.ipynb
├── Polynomial Regression/
│   ├── polynomial_regression.ipynb
│   ├── euro12.ipynb
│   └── Position_Salaries.csv
├── Spam Classifier/
│   ├── Spam_Bayesian_Inference_.ipynb
│   └── SMSSpamCollection
├── SQL Projects/
│   └── COVID Portfolio Project - Data Exploration.sql
├── SVR/
│   ├── support_vector_regression.ipynb
│   └── Position_Salaries.csv
├── Web Scraping/
│   └── Amazon Web Scraper Project.ipynb
├── PJME_hourly.csv
├── pjme_time_series_analysis.ipynb
└── time_series_forecasting.ipynb
```

---

*Built with Python, scikit-learn, XGBoost, and Jupyter Notebooks.*
