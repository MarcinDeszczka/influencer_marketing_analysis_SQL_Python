# Influencer Marketing Performance Analysis

A portfolio project focused on **marketing analytics**, combining **SQL and Python** to analyze influencer marketing campaign performance, influencer effectiveness, ROI, customer behavior, and revenue trends.

## Project Overview

Welcome to my portfolio!

I am **Marcin Deszczka**, a data analyst specializing in marketing analytics.

For this project, I selected the synthetic **[Influencer Marketing Campaign Analysis](https://www.kaggle.com/datasets/divyamehulmak/influencer-marketing-campaign-analysis-power-bi/)** dataset from Kaggle and independently prepared the data for SQL and Python analysis.

The project focuses on practical analytical tasks such as:

* influencer segmentation and data consistency checks,
* campaign performance analysis,
* influencer performance profiling,
* identifying influencers performing above average,
* ROI benchmarking by platform,
* month-over-month revenue analysis,
* product category effectiveness,
* revenue flow visualization.

## Dataset

The dataset represents a synthetic but realistic simulation of influencer marketing campaigns in the fashion industry. It contains data covering influencers, campaigns, products, orders, and customer demographics.

### Main tables

* **Influencers** — 20 unique influencers, including follower count, platform, tier, location, engagement, and audience demographics.
* **Campaigns** — 10 campaigns containing budget, duration, product category, primary goal, and platform.
* **Products** — 25 products with categories, subcategories, target gender, seasonality, pricing, and launch dates.
* **Orders** — more than 100,000 records connecting customers, products, influencers, campaigns, discount codes, and generated revenue.
* **Customer Demographics** — more than 90,000 unique customers, including age, gender, location, income bracket, preferred style, new-customer status, and Customer Lifetime Value (CLV).

The dataset makes it possible to analyze campaign effectiveness, revenue generation, influencer performance, customer segmentation, and purchasing patterns.

> **Note:** The dataset is synthetic and intended for demonstration purposes. Financial figures, including ROI, may therefore appear unrealistic. This does not affect the analytical methodology. All financial values are treated as being denominated in **US dollars (USD)**.

## Data Preparation

The SQL and Python analyses use the same original Kaggle source, but the data were prepared independently for each environment.

### SQL

For the SQL analysis, the original `.xlsx` data were converted to `.csv` and then imported into an SQLite `.db` database using DB Browser for SQLite.

During the process, I manually checked the imported data and corrected incorrect data types. I then used Python to replace incorrectly converted commas with decimal points where necessary.

### Python

For the Python analysis, the original `.xlsx` files were loaded directly.

This approach allowed me to work with the same source data while independently preparing the datasets for two different analytical environments.

## Technologies

The project combines two complementary approaches:

### SQL

* SQLite
* DB Browser for SQLite
* Jupyter Notebook
* SQL queries executed using `%%sql`

The SQL analysis was written entirely by me.

### Python

* Python
* pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* openpyxl
* IPython.display
* re

Jupyter Notebook was used as the main environment for combining code, analysis, visualizations, and results.

I also used AI tools as an auxiliary resource during the project, primarily for assistance with technical questions and development.

## Analysis

### Part I — SQL

1. **Influencer Segmentation — Data Consistency Audit**
2. **Campaign Aggregation**
3. **Comprehensive Influencer Performance Profile**
4. **Creator Selection Above Average**
5. **ROI Benchmark by Platform**
6. **Month-over-Month (MoM) Revenue Trend**

### Part II — Python

7. **Impact of Product Category on Campaign Effectiveness**
8. **Revenue Flow Visualization (Sankey)**

The complete analysis, SQL queries, Python code, visualizations, and conclusions are available in the accompanying Jupyter Notebook.

## Project Structure

```text
Python_SQL/
│
├── README.md
├── README_PL.md
│
├── influencer_marketing_analysis_EN.ipynb
├── influencer_marketing_analysis_PL.ipynb
│
│
└── ...
```

## Purpose

This project was created as part of my **data analytics portfolio** to demonstrate practical skills in:

* SQL querying and data aggregation,
* CTEs and window functions,
* data quality verification,
* data cleaning and preparation,
* exploratory data analysis,
* marketing analytics,
* ROI analysis,
* data visualization,
* translating business questions into analytical queries.

The project is intended as a demonstration of analytical methodology rather than a representation of real-world financial performance.
