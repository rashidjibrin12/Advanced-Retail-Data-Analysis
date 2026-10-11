# Advanced Retail Data Analysis

## Project Overview
This project analyzes the Online Retail II dataset to understand customer purchasing behavior, identify high-value segments, and assess opportunities for retention and revenue growth. The analysis goes beyond aggregate sales trends by examining customer-level patterns in recency, frequency, and monetary value.

The notebook cleans the transactional data, builds a customer-level RFM model, and applies K-means clustering to segment the customer base into meaningful groups. The goal is to translate raw retail transaction data into actionable business insights that inform marketing, loyalty, and retention strategy.

## Why This Analysis Matters
The project is designed to answer practical retail questions such as:
- Which customers generate the most revenue?
- Which customers are most at risk of churn?
- Which segments are most responsive to retention campaigns?
- How should marketing spend be prioritized across customer groups?

## Dataset and Business Context
The analysis uses the Online Retail II dataset, which contains transaction-level records for online retail purchases, including invoice information, product descriptions, quantities, prices, customer IDs, and country data.

Key fields include:
- Invoice number and date
- Stock code and product description
- Quantity and unit price
- Customer ID
- Country
- Total order value

A key observation from the data is that the business is highly concentrated in the United Kingdom, with a long tail of customers in other markets. This concentration matters because it suggests that the strongest revenue and retention opportunities are likely tied to the core UK customer base, while international buyers are more fragmented and lower-volume.

## Data Cleaning and Preparation
The notebook applies a structured data-cleaning workflow before modeling:
- removes records with missing customer IDs
- filters out cancelled or invalid transactions
- removes negative or zero quantity and price entries
- eliminates duplicate records
- creates a total sales value feature for each transaction
- converts invoice dates to datetime for time-based analysis

This preprocessing step ensures the cluster and RFM analysis reflects valid customer behavior rather than transaction anomalies or return activity.

## Core Analytical Approach
The project uses a standard customer analytics workflow:
- RFM analysis to evaluate customer recency, frequency, and monetary value
- StandardScaler to normalize RFM features before clustering
- K-means clustering to group customers into business-relevant segments
- Customer segmentation visualization to interpret cluster behavior

This approach helps turn transaction history into customer-level strategic insight instead of relying only on raw sales totals.

## Key Findings
The analysis reveals several important findings for the retail business:

- Revenue is not evenly distributed across customers: a relatively small group of customers contributes a large share of total sales.
- Recency, frequency, and monetary value are strong indicators of customer engagement and profitability.
- Customers with recent purchases and repeated buying behavior are the most valuable segments for retention and upselling.
- Inactive or low-frequency customers represent the clearest opportunity for reactivation campaigns.
- The dataset shows a strong UK market concentration, which suggests that marketing and retention strategies may be most effective when tailored to the dominant domestic segment.
- K-means clustering identifies multiple customer archetypes with distinct spending and engagement profiles, supporting more targeted customer strategy.

## Customer Segmentation Insights
The clustering results identify several customer segments, including:
- high-value, frequent buyers who drive revenue and repeat purchases
- active but lower-value customers who may respond to cross-sell or loyalty programs
- low-frequency or inactive customers who are at higher churn risk
- occasional buyers with limited revenue contribution but potential for reactivation

These segment patterns help move the analysis from descriptive reporting to actionable customer strategy.

## Business Impact
This project demonstrates how transactional data can be converted into customer-level intelligence that supports better decision-making across marketing, CRM, and revenue planning.

The findings suggest that the business should:
- prioritize retention and loyalty strategies for its highest-value customers
- design re-engagement campaigns for inactive or low-frequency accounts
- focus acquisition and promotional spend where customer value is strongest
- use segmentation to personalize offers instead of applying one-size-fits-all promotions

## Tools and Technologies
- Python
- pandas for data wrangling and transformation
- NumPy for numerical analysis
- Matplotlib for visual storytelling
- Seaborn for statistical visualization
- scikit-learn for clustering and segmentation
- Jupyter Notebook for reproducible analysis
- Kaggle dataset sourcing and notebook-based reporting

## Portfolio Summary
This project showcases the ability to work with real-world transactional data, clean and structure retail records, apply customer analytics methods, and translate model outputs into business-ready recommendations. It reflects a practical, decision-oriented approach to data analysis where insights are tied directly to retention, customer value, and revenue strategy.
