**Olist E-Commerce Sales & Customer Analytics**

**1. Project Overview**

This project analyzes the Brazilian Olist E-Commerce dataset using Microsoft Power BI to understand sales performance, customer behaviour, payment preferences, and delivery efficiency.

**2. Business Problem Statement**

E-commerce businesses generate large volumes of transactional data. Without proper analysis, it is difficult to monitor sales performance, understand customer behaviour, and identify delivery issues.

This project transforms raw e-commerce data into meaningful business insights through interactive Power BI dashboards.

**3. Business Questions**

1. What is the total revenue and number of orders?
2. How does revenue change monthly?
3. Which product categories generate the highest revenue?
4. Which payment methods are most commonly used?
5. What is the average delivery time?
6. How satisfied are customers based on review scores?
7. How does performance vary by year, product category, and customer state?

**Data Cleaning and Preparation**

Data cleaning and preparation were performed using Power Query in Power BI.

The following steps were completed:

- Imported the Olist e-commerce datasets into Power BI.
- Verified and corrected column data types, including dates, numbers, and text.
- Checked missing values in important columns.
- Preserved legitimate null values in delivery-related date columns where orders had not been delivered.
- Checked duplicate records in key columns.
- Validated composite keys in order items and payment datasets.
- Created a cleaned geolocation reference table by removing duplicate records while preserving the original table.
- Reviewed product and review data to ensure valid records were not incorrectly removed.
- Applied and loaded the cleaned datasets into Power BI for data modelling and analysis.

**Data Model and Relationships**

A relational data model was created in Power BI to connect the different e-commerce datasets and support accurate analysis.

The data model includes the following relationships:

- Customers → Orders
- Orders → Order Items
- Orders → Payments
- Orders → Reviews
- Products → Order Items
- Sellers → Order Items
- Product Category Translation → Products

The relationships were configured using the appropriate key columns and cardinality to enable filtering and analysis across the datasets.

The model supports analysis of sales performance, customer behaviour, product categories, payment methods, reviews, and delivery performance.

## DAX Measures

The following DAX measures were created to calculate key business metrics and support dashboard analysis:

| Measure | Purpose |
|---|---|
| Total Revenue | Calculates total product sales revenue |
| Total Orders | Counts distinct orders |
| Total Customers | Counts unique customers |
| Average Order Value | Calculates average revenue per order |
| Monthly Revenue | Tracks revenue trends over time |
| Total Payment Value | Calculates total recorded payment value |
| Average Delivery Days | Measures average delivery time for completed orders |
| Average Review Score | Calculates average customer review rating |
| Review Count | Counts customer reviews |

These measures help monitor business performance and identify trends in sales, customer satisfaction, and delivery efficiency.

**Note:** Total Revenue is calculated using product item prices and excludes freight charges. It represents sales value, not profit.

**4. Tools Used**

- Microsoft Power BI
- Power Query
- DAX
- Brazilian Olist E-Commerce Dataset


**5. Dashboard Overview**

**Page 1: Sales Performance**
- Total Revenue
- Total Orders
- Total Customers
- Average Order Value
- Monthly Revenue Trend
- Revenue by Product Category
- Payment Method Distribution

**Page 2: Customer & Delivery Analysis**
- Average Review Score
- Customer Review Score Distribution
- Monthly Average Delivery Time
- Customer State Filter

**6. Key Business Insights**

 1. Revenue Performance: The business generated total revenue of R$13.59 million across 99,441 orders.

 2. Average Order Value: The average order value was R$136.68, indicating the average item-price revenue per order.

 3. Customer Base: The analysis identified 96,096 unique customers, providing a broad customer base for the e-commerce business.

 4. Customer Satisfaction: The average review score was 4.09 out of 5. The majority of reviews received 5 stars (57,328 reviews), indicating generally positive customer feedback.

 5. Review Distribution: There were 19,142 four-star reviews and 11,424 one-star reviews. These lower ratings provide opportunities to investigate customer dissatisfaction.

 6. Product Category Performance: Revenue varied across product categories, with clear differences between the highest- and lower-revenue categories.

 7. Payment Preferences: Credit card payments represented the largest share of payment value in the dashboard.

 8. Revenue Trends: Monthly revenue analysis highlights changes in sales performance over the dataset period.

**7. Business Recommendations**

 1. Improve Customer Experience: Investigate one-star and two-star reviews to identify recurring complaints and improve customer satisfaction.

 2. Increase Average Order Value: Consider product bundles, cross-selling, and targeted promotions to encourage customers to purchase additional products.

 3. Optimize Product Category Performance: Focus marketing and inventory planning on high-revenue product categories while investigating opportunities to improve lower-performing categories.

4. Improve Delivery Efficiency: Investigate months with longer average delivery times and identify potential logistics bottlenecks.

5. Maintain Payment Convenience: Continue supporting popular payment methods and ensure a smooth payment experience.

6. Monitor Monthly Revenue: Track monthly sales trends and plan promotional campaigns during weaker sales periods.

**8. Conclusion**

This project demonstrates the use of Power BI to transform e-commerce data into interactive dashboards and actionable business insights.

**POWER BI DASHBOARD**

Download the Power Bi dashboard from [Github Releases](https://github.com/kpriyadharshini0102-eng/olist-ecommerce-sales-analytics/releases/tag/v1.0) section.

The dashboard contain two pages:
 -- Sales Performance
 -- Customer & Delivery Analysis
