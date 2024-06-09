# BCG X Data Science Job Simulation
BCG X Data Science Job Simulation - use data to advise PowerCo, on how to retain their customers with the team at BCG X. (https://www.theforage.com/simulations/bcg/data-science-ccdz)
## 1. Background
### 1.1 Client
  - Power Co, a major gas and electricity utility who is concerned about losing customers
  - Main clients are small and medium sized enterprises
  - The energy market has had a lot of change recent years and there are more options than ever for customers to choose them

### 1.2 Characteristics about the industry
  - Low level of differentiation between products available to customers
  - Customer service being a top priority
  - Keeping customers for long term and building brand loyalty

### 1.3 Goal
investigate the reason for Power Co's clients switching to another service provider (customer churn)


## 2. How to run
### 2.1 Setup
Ensure some important python packages are installed on your system.

> pandas, numpy, matplotlib.pyplot, seaborn, datetime, dateutil.relativedelta, relativedelta

### 2.2 Running the Code
Those 2 python could run directly if system environment is done. Should be careful when setting the file path.


## 3. How it works
### 3.1 EDA
Descriptive statistics analysis of data, Data visualization - Univariate Analysis, Bivariate Analysis, Hypothesis Investigation (correlation)

### 3.2 Feature Engineering
1. Create new variables based on project background
   - Difference between off-peak prices in December and preceding January
   - Average price changes across periods, Max price changes across periods
   - Tenue
2. Transforming dates into months
   - Dates as a datetime object are not useful for a predictive model, so we needed to use the datetimes to create some other features that may hold some predictive power.
    
3. Handle & Transform categorial data; data cleaning
   - One hot encoding using get_dummies()

4. Handle & Transform numeric data
   - Handle Skewness; perform log10 transformation

5. Correlation Analysis

### 3.3 Build predictive models
1. Data Preprocessing - SMOTE
2. Logistic Regression (with Lasso penalty)
3. Random Forest

