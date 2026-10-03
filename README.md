# Advanced Retail Data Analysis — Online Retail II

This repository contains my exploratory and advanced analysis of the "Online Retail II" transactional dataset. I analyzed the uploaded Jupyter notebook (Online_Retail_II.ipynb) to clean the data, extract insights about customers and products, and build advanced models that support customer segmentation, forecasting, and product analysis.

## Contents

- Online_Retail_II.ipynb — Jupyter notebook with the full analysis and visualizations (uploaded by repository owner)
- README.md — this file
- requirements.txt — (recommended) Python packages used to reproduce the notebook


## Summary of analysis performed

1. Data loading and initial inspection
   - Loaded the Online Retail II dataset and inspected schema, missing values, and basic summary statistics.
   - Converted date/time fields to pandas datetime, and ensured correct dtypes for numeric fields.

2. Data cleaning and preprocessing
   - Removed transactions with missing or invalid CustomerID where appropriate.
   - Filtered out cancellations and negative quantities and removed extreme outliers in UnitPrice and Quantity.
   - Created a clean transactional master table and derived invoice-level and customer-level aggregates.

3. Exploratory Data Analysis (EDA)
   - Sales trend analysis by day/week/month, seasonal patterns, and moving averages.
   - Top products by revenue and quantity sold; long-tail analysis of SKUs.
   - Geographic breakdown of sales and visualization of country-level contributions.

4. Customer-level analytics
   - RFM analysis (Recency, Frequency, Monetary) to score and segment customers into groups (Loyal, At-risk, etc.).
   - Created RFM score bands and visualized segment distributions.
   - Customer cohorts by first purchase month and retention rate visualization.

5. Segmentation and clustering
   - Scaled RFM features and applied KMeans clustering to identify distinct customer segments.
   - Validated cluster count using the elbow method and silhouette scores, and profiled each cluster.

6. Time series and forecasting
   - Aggregated revenue and order counts into daily and weekly series.
   - Decomposed series into trend/seasonality and used forecasting models to project short-term revenue.
   - Evaluated forecasts with holdout sets and common metrics (MAE, RMSE, MAPE).

7. Customer Lifetime Value (CLTV) and churn modeling
   - Implemented simple CLTV estimation using historical monetary and frequency metrics to predict future customer value.
   - Explored churn indicators and simple churn prediction models using logistic regression and tree-based models.

9. Advanced models and diagnostics
   - Built baseline predictive models for high-value customer identification, next-best product recommendations, and purchase propensity.
   - Evaluated models with cross-validation and confusion metrics where applicable.

10. Visualizations and reporting
    - Interactive charts for product dashboards and static visualizations (Matplotlib/Seaborn) for reports.
    - Notebook contains annotated charts and markdown explaining findings and business implications.



