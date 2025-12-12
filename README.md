RFM Customer Segmentation Dashboard (Tableau)
📌 Project Overview

This project presents an RFM (Recency, Frequency, Monetary) Analysis Dashboard built using Tableau to analyze customer purchasing behavior and segment customers based on engagement and value.

🧹 Data Cleaning & Preparation (Jupyter Notebook)

Before building the Tableau dashboard, the dataset was cleaned and prepared using Python in Jupyter Notebook to ensure accuracy, consistency, and reliability of the analysis.

📌 Data Sources

The analysis was performed on multiple customer-related datasets, including:

Transaction data

Customer demographic information

Customer address data

New customer records

These datasets were merged and transformed into a unified customer-level table for RFM analysis.

🔧 Data Cleaning Steps Performed

The following preprocessing steps were carried out using Pandas:

1️⃣ Handling Missing Values

Removed records with missing or invalid customer identifiers.

Handled missing monetary and frequency values appropriately to avoid skewed results.

2️⃣ Date Processing

Converted transaction date columns to proper datetime format.

Calculated Recency as the number of days since the customer’s last purchase using a fixed reference date.

3️⃣ Aggregation at Customer Level

Grouped transaction-level data by Customer ID.

Computed:

Recency: Days since last transaction

Frequency: Total number of transactions

Monetary: Total spend per customer

4️⃣ Outlier and Data Consistency Checks

Validated frequency and monetary ranges to identify abnormal values.

Ensured all RFM metrics were positive and logically consistent.

5️⃣ RFM Scoring

Divided Recency, Frequency, and Monetary values into quartiles.

Assigned R, F, and M scores to each customer.

Combined scores to create meaningful RFM segments (Champion, Loyal, At Risk, etc.).

6️⃣ Export for Visualization

Final cleaned and aggregated dataset was exported as a CSV file.

This dataset was then used directly in Tableau for visualization and dashboard creation.

<img width="1295" height="797" alt="image" src="https://github.com/user-attachments/assets/4c461c20-d132-4a7f-9152-607439e46917" />

The dashboard helps answer key business questions such as:

Who are our most valuable customers?

Which customers are at risk of churn?

How does spending relate to purchase frequency and recency?

The analysis enables data-driven decision-making for marketing strategy, customer retention, and revenue optimization.

📈 Key Performance Indicators (KPIs)

The top section of the dashboard displays high-level KPIs that summarize customer behavior:

🔹 Total Customers

Represents the total number of unique customers included in the analysis.

Provides context for all subsequent distributions and segments.

🔹 Average Monetary Value

Average total spending per customer.

Helps assess overall customer value and revenue contribution.

🔹 Average Frequency

Average number of purchases per customer.

Indicates how often customers engage with the business.

🔹 Average Recency

Average number of days since the customer’s last purchase.

Lower values indicate more recent customer engagement.

📊 Distribution Analysis
1️. Recency Distribution Histogram

What it shows:

Distribution of customers based on how recently they made a purchase.

Why it matters:

Identifies active vs inactive customers.

A large concentration at lower recency values indicates a healthy, engaged customer base.

Insight:

Most customers have purchased recently, while a smaller group shows long inactivity, representing churn risk.

2️. Frequency Distribution Histogram

What it shows:

Distribution of customers based on the number of purchases made.

Why it matters:

Helps identify repeat buyers versus one-time customers.

Indicates customer loyalty patterns.

Insight:

Majority of customers fall within moderate frequency ranges, with fewer high-frequency loyal customers.

3️. Monetary Distribution Histogram

What it shows:

Distribution of total spending per customer.

Why it matters:

Highlights spending behavior and revenue concentration.

Helps identify high-value customers.

Insight:

Most customers fall into mid-range spending, while a small segment contributes significantly higher revenue.

🔗 Relationship Analysis
4️. Recency vs Monetary Scatter Plot

What it shows:

Relationship between how recently a customer purchased and how much they spend.

Why it matters:

Helps identify high-spending customers who may be disengaging.

Useful for targeted reactivation campaigns.

Insight:

Customers with lower recency tend to have higher monetary values, indicating recent high-value buyers.

5️. Frequency vs Monetary Scatter Plot

What it shows:

Relationship between purchase frequency and total spending.

Why it matters:

Validates that frequent customers tend to spend more.

Helps identify loyal, high-value customers.

Insight:

Clear positive correlation between frequency and monetary value, reinforcing loyalty-driven revenue growth.

🧩 Customer Segmentation (RFM Segments)

6️. RFM Segment Bar Chart

Customers are segmented based on their combined RFM scores into meaningful business categories:

Champion – Recent, frequent, high spenders

Big Spender – High monetary value customers

Loyal – Frequent repeat customers

Potential Loyalist – Customers with growth potential

At Risk – Previously active but now disengaging

Regular – Average engagement customers

Why it matters:

Enables targeted marketing strategies.

Helps prioritize retention and upselling efforts.

Insight:

The largest group consists of Regular and At Risk customers, highlighting opportunities for engagement and retention campaigns.

🎯 Business Use Cases

Customer retention strategy

Personalized marketing campaigns

Revenue optimization

Loyalty program design

🛠 Tools & Technologies

Python, Jupyter Notebook

Tableau – Data visualization and dashboard creation

Excel / CSV – Cleaned data sources

RFM Analysis Framework – Customer segmentation methodology
