# Advanced Retail Data Analysis

## Project Overview
This project analyzes the Online Retail II dataset to understand customer purchasing behavior, identify high-value segments, and assess opportunities for retention and revenue growth. The analysis goes beyond descriptive sales reporting by focusing on customer value, retention risk, and business segmentation.

The notebook cleans the transactional data, builds a customer-level RFM model, and applies K-means clustering to segment the customer base into meaningful groups. The goal is to translate raw retail transaction history into practical insight for revenue growth and customer retention strategy.

## Why This Analysis Matters
The project is designed to answer practical retail questions such as:
- Which customers generate the most revenue?
- Which customers are most at risk of churn?
- Which segments are most responsive to retention campaigns?
- How should marketing spend be prioritized across customer groups?

## Tools and Technologies
- Python
- Pandas for data wrangling and transformation
- NumPy for numerical analysis
- Matplotlib for visual storytelling
- Seaborn for statistical visualization
- Scikit-learn for clustering and segmentation
- Jupyter Notebook for reproducible analysis
- Kaggle dataset sourcing and notebook-based reporting

## Dataset and Business Context
The analysis uses the Online Retail II dataset, which contains transaction-level records for online retail purchases, including invoice information, product descriptions, quantities, prices, customer identifiers, and country information.

Key fields include:
- Invoice number and date
- Stock code and product description
- Quantity and unit price
- Customer ID
- Country
- Total order value

A key observation from the data is that the business is highly concentrated in the United Kingdom, with a long tail of customers in other markets. This concentration matters because it suggests that marketing and retention strategies may need to be more tailored for the largest domestic segment while still accounting for smaller international opportunities.

## Data Cleaning and Preparation
The notebook applies a structured data-cleaning workflow before modeling:
- Removes records with missing customer IDs
- Filters out cancelled or invalid transactions
- Removes negative or zero quantity and price entries
- Eliminates duplicate records
- Creates a total sales value feature for each transaction
- Converts invoice dates to datetime for time-based analysis

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

---

## Visualizations

### Customer Segmentation Analysis

<img width="700" height="500" alt="Customer Segmentation Clusters" src="https://github.com/user-attachments/assets/2d7bf44b-a759-4e15-b35f-98d79c4e02a4" />

<br/><br/>

<img width="700" height="500" alt="RFM Analysis Visualization" src="https://github.com/user-attachments/assets/273e9fe7-5448-4597-8f7c-528c979a3058" />

<br/><br/>

<img width="700" height="500" alt="Customer Value Distribution" src="https://github.com/user-attachments/assets/56e38d4d-8716-4027-b7fa-382597a8510f" />

<br/><br/>

---

## Customer Segmentation Insights
The clustering results identify several customer segments, including:
- High-value, frequent buyers who drive revenue and repeat purchases
- Active but lower-value customers who may respond to cross-sell or loyalty programs
- Low-frequency or inactive customers who are at higher churn risk
- Occasional buyers with limited revenue contribution but potential for reactivation

These segment patterns help move the analysis from descriptive reporting to actionable customer strategy.

## Business Impact
The findings suggest that the business should:
- Prioritize retention and loyalty strategies for its highest-value customers
- Design re-engagement campaigns for inactive or low-frequency accounts
- Focus acquisition and promotional spend where customer value is strongest
- Use segmentation to personalize offers instead of applying one-size-fits-all promotions

---

## About Me
**Abdulrashid Jibrin**

Aspiring Data Analyst | SQL & Power BI | AI tools and ML
