# Suspermarket Sales Analysis (SSA)
This notebook will use SQL to analyse a [supermarket database](https://www.kaggle.com/datasets/lovishbansal123/sales-of-a-supermarket) using branch information, customer data, product data, revenue. 

## Objectives
The objective of this project is to introduce basic ideas of:
- How to extract data?
- Mathematical operations inside queries
- Ordering data based on business questions
- Create conditions

## Business Questions
### 1. General Sales Analysis
- What is the total revenue generated by the supermarket across all branches?
- Which branch generates the highest revenue?
- How many transactions were made in each branch?

SQL Skills:
- Basic `SELECT`, `SUM`, `GROUP BY`, and `ORDER BY`.

### 2. Customer Behavior
- What is the average spending per customer?
- Which customer group (e.g., loyalty vs. non-loyalty) spends the most on average?
- How many loyal customers in each branch?
- What are the top 3 products by revenue in each branch?

SQL Skills:
- Use of aggregate functions like `AVG` and `COUNT`.
- Mathematical operations in queries.

### 3. Product Performance
- Which product category generates the most revenue?
- What is the best-selling product in each branch?
- How does the revenue of each product category compare between branches?

SQL Skills:
- Aggregations with `SUM` and `GROUP BY`.
- `WHERE` for conditioning.
- `ORDER BY`and `RANK` for ranking.

### 4. Revenue Trends
- What is the revenue trend over time (e.g., by day, week, or month)?
- Which day of the week has the highest sales?

SQL Skills:
- Date manipulation and grouping (`DATE`, `EXTRACT`, `GROUP BY`).
- Conditions with `CASE`.

### 5. Operational Insights
- What is the Cost of Goods (CoG) per product??
- What is the network net profit?
- What is the distribution of payment methods (e.g., cash, credit card)?

### Stretch Questions (for Intermediate Exploration)
- What is the profit margin for each product category?
- What are the top 3 products by revenue in each branch?