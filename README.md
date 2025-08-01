global-happiness-analysis/
|
├── data/                      # Raw & processed data
│   ├── 2015.csv
│   ├── 2016.csv
│   ├── 2017.csv
│   ├── 2018.csv
│   ├── 2019.csv
│   └── concat_updated.xlsx    # Cleaned and merged dataset
│
├── notebooks/                # Jupyter notebooks for analysis
│   ├── 01_EDA.ipynb          # Exploratory Data Analysis
│   └── 02_Regression_Model.ipynb  # Linear Regression modeling
│
├── powerbi/                  # Replaced by Tableau dashboard
│   └── happiness_dashboard.twb
│
├── outputs/
│   ├── figures/              # Exported graphs and plots
│   └── reports/              # Additional visual assets
│
├── README.md                 # Project overview (this file)
└── requirements.txt          # Python dependencies









🔍 Dataset Overview

The World Happiness Reports (2015-2019) provide annual data from Gallup World Poll surveys, capturing variables such as GDP, social support, freedom, trust in government, generosity, and life expectancy.

Source: Kaggle / World Happiness Report

Combined dataset size: ~800 rows across 5 years

Unified structure with 11 standard columns + year indicator

📊 Analysis Process

1. Data Cleaning & Preparation

Normalized inconsistent column names across years

Combined all data into one structured dataset

Added missing Region values via country mapping

Removed Dystopia Residual due to data absence in 2018/2019

2. Exploratory Data Analysis (EDA)

Analyzed missing values, feature distributions

Checked feature relationships with Score

Visualized variable distributions and correlations

3. Regression Modeling

Built a Linear Regression model to predict Happiness Score

Evaluated performance with R²: 0.602 and RMSE: 0.644

Key contributing factors:

Freedom (1.48 coef)

Social Support (1.23 coef)

Trust (1.11 coef)

4. Visualization with Tableau

Replaced original Power BI plan due to login restrictions.

Dashboard Pages:

Page 1: Happiness Overview

Average happiness score (Card)

Scores by country (Bar Chart)

Regional averages (Column Chart)

Top 10 & bottom 10 countries (Donut & Bar Charts)

Page 2: What Drives Happiness?

Scatter plots: Score vs GDP, Freedom, Trust

Correlation grid (manually constructed)

Page 3: KPI & Insights

Highest GDP country (💰)

Highest happiness with lowest GDP (🧠)

Most trusted country (🛡)

Most socially supportive country (👥)



🚀 Skills Demonstrated

Data cleaning, transformation and feature engineering

Exploratory Data Analysis (EDA) using pandas, matplotlib, seaborn

Machine learning with scikit-learn

Tableau dashboard creation and KPI visualization

Project structuring and documentation

📆 Timeline

Project Duration: ~7 days (Titanic-style walkthrough)

Tools: Jupyter, Python, Tableau Public

Dataset Language: English

📥 How to Run This Project

Clone this repo

Install dependencies: pip install -r requirements.txt

Run Jupyter notebooks in order:

01_EDA.ipynb

02_Regression_Model.ipynb

Open happiness_dashboard.twb in Tableau to explore dashboards