# Customer Segmentation Analysis Report
Discover sales trend and customer behavior from 2019 to 2024

# Introduction & Background
The goal of this analysis project is to track customer behavior, analyze sales trends, and assess product performance across different countries. This analysis will help industries improve their sales and marketing strategies while gaining a deeper understanding of customer preferences and behaviors. Additionally, this dashboard provides key performance indicators (KPIs) that stakeholders can use to support data-driven decision-making.

This project also serves as a demonstration of my expertise in data analysis, specifically in using SQL and Google BigQuery.

# Business Objectives

This report aims to answer the following business questions:

- What are the total order sales, revenue, cost of goods sold (COGS), and gross profit?
- What is the gross margin? Is it increasing or decreasing?
- How does revenue vary by year, quarter, and gender?
- What are the top three revenue-generating products and brands?
- How do sales vary by time of day and day of the week (weekend vs. weekday)?
- What is the breakdown of sales by order status (e.g., shipped, completed, returned)?
- How does current revenue compare to the target?
- What is the total number of orders, and how many were placed this month?
- What is the percentage of repeat customers?
- Who are the top three revenue-generating customers?
- What is the total number of users and customers?
- What is the distribution of customers by recency, engagement level, and number of failed orders?
- Which browser is most commonly used by customers?
- What are the top-selling products by revenue?
- What are the top brands by revenue?


# Data Source & Methodology

**Data Source:**
The datasets used in this analysis were sourced from the **Google BigQuery Platform**. The same datasets are also available on Kaggle (“kaggle.com”). SQL queries were used to extract relevant data, which was then exported as a CSV file. Unnecessary and redundant columns were excluded to streamline the analysis.

**Data Cleaning & Transformation:**
- Used data profiling tools to detect and correct anomalies.
- Replaced values to ensure correct date and time formatting (e.g., order date, return date, and ship date).
- Split date and time into separate columns for better time intelligence analysis.
- Merged two related tables (**Orders** and **Order Items**) to consolidate order quantity data.
- Ensured all data types were correctly formatted to prevent discrepancies.

**Data Model:**

- The dataset follows a **snowflake schema**, making the analysis slightly complex. However, with proper modeling, it aligns well with the business objectives.

- Set cross-filter relationships to **single** to avoid ambiguity and unnecessary complexity in data relationships.


**Analysis Approach:**

- Created **date and time lookup** tables for more precise time-based analysis.

- Used **DAX (Data Analysis Expressions)** to create complex measures, calculated columns, and calculated tables. Examples include top three customers by revenue, repeat customer percentage, and sales comparisons.

# Dashboard Features & KPIs

**Key Metrics:**
- **Total Users**
- **Total Customers**
- **Repeat Customer Percentage**
- **Total Completed Orders**
- **Total Returned Orders**
- **Total Sales**
- **Total Revenue**
- **Total COGS**
- **Gross Profit**
- **Gross Margin**

**Visualizations:**

- **Line Graph:** Displays total sales and revenue trends over time (by year and date hierarchy).
- **Pie Chart:** Shows the distribution of total user events by browser.
- **Bar Graph:** Highlights the top three revenue-generating products.
- **Map:** Visualizes sales distribution across different countries.
- **Table:** Displays customer behavior details, such as purchase frequency, recency, engagement level, and failed orders.

# Conclusion & Recommendation

**Summary:**

- The **e-commerce platform** has a total of **100,000 registered users**, of which **80,000 are customers**.
- **Repeat customers** account for **24.78%** of total purchases.
- The platform generated a **total revenue of $5 million**, with a **gross profit of $3 million** (51.91% profit margin).
- Sales are significantly higher on **weekdays** (72%) compared to weekends (28%).
- The total number of orders is **182,000**, with **46,000 completed orders** and **18,000 returned orders** (10.13% return rate).
- The **top three revenue-generating products** are:
    - **The North Face Apex Bionic Soft Shell Jacket** – $19,866
    - **Nike Women’s Pro Compression Sports Bra** – $11,739
    - **The North Face Apex Bionic Men’s Soft Shell Ski Jacket 2013** – $9,933
      
- The **year 2023** recorded the highest **total sales ($9.66 million)** and **total revenue ($2.43 million)**, contributing to a 33.3% profit growth compared to previous years.

**Recommendations:**

- **Revenue Conversion Issues:** Despite the significant increase in sales in 2023, a large portion did not convert into revenue. A deeper analysis is needed to understand potential factors, such as pricing strategy, discounting policies, or operational costs. Conducting a **customer feedback analysis** could help identify revenue leakage points.
- **User Engagement vs. Purchases:** Many users interact with the platform but do not complete purchases. Further analysis is required on **user behavior metrics** (e.g., clicks, add-to-cart actions, checkout abandonment). Offering discounts or promotional vouchers may help convert engaged users into customers.
- **High Return Rate:** The **return rate of 10.13% ($2 million loss in sales)** requires investigation. Collecting **product reviews**, **delivery feedback**, and **customer complaints** can provide insights into return reasons (e.g., defective items, misleading product descriptions, or shipping issues).
- **Uncompleted Shipments:** There are many **orders marked as shipped but not completed**. The reasons could be **logistics delays** or **system errors** in order processing. Further investigation into supply chain inefficiencies or platform glitches is needed to ensure timely order fulfillment.

# Dashboard

![image](https://github.com/user-attachments/assets/260b606f-4e43-4d6a-a9f0-350acf2f9a5e)

![image](https://github.com/user-attachments/assets/5fdde560-b909-43c8-ba8a-0a8e30c103ec)


