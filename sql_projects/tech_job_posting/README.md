![Alt text](https://images.unsplash.com/photo-1508780709619-79562169bc64?q=80&w=1740&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

# Tech Job Posting (TJP)
This project explores datasets related to data science job salaries, job postings, and required skills to analyze salary trends, skill demand, and industry opportunities. Using advanced SQL techniques, the project focuses on integrating data from multiple tables to uncover valuable insights into the global job market for data professionals.

I'm using free datasets on Kaggle:
- [LinkedIn Job Postings (2023-2024)](https://www.kaggle.com/datasets/arshkon/linkedin-job-postings)

## **Advanced SQL Techniques**
This project employs advanced SQL techniques such as:  
- **JOINs**: INNER, LEFT, and FULL OUTER to integrate datasets.  
- **CTEs**: To simplify complex queries and identify skill trends.  
- **Window Functions**: For ranking and tracking industry growth.  
- **Aggregations**: To summarize salary and job data.  
- **Subqueries**: To isolate and filter niche data points.

## Objective
- Analyze salary patterns by job title, location, and experience level.
- Explore the demand for technical skills across industries and company sizes.
- Identify the impact of remote work on salaries and job opportunities.
- Uncover trends in emerging industries hiring data professionals.

## **Business Questions**
### 1. Salary Trends and Insights
- What is the average salary for data science jobs across different industries?
- How do company sizes impact the salaries offered for data science roles?
- Which job titles offer the highest average salary for data professionals?

SQL Skills:
- JOINs (INNER JOIN between job_postings, job_industries, and companies to connect salary, industry, and company data).
- Aggregations (AVG to calculate averages and trends over time).

### 2. Skill Demand and Growth
- Which skills are most in demand for data science roles globally?
- How do industry types influence the demand for specific data science skills?
- What skills are associated with the highest paying data science roles?

SQL Skills:
- CTEs (to simplify queries that identify and track specific skill sets over time).
- JOINs (to link job_skills, job_postings, and company_industries to analyze skill trends).
- Aggregations (COUNT, GROUP BY to identify the frequency of specific skills in job postings).

### 3. Company Overview and Job Postings Analysis
- Which companies post the most data science jobs?
- How does the size of a company correlate with the number of job postings?
- What are the top industries for data science job postings?

SQL Skills:
- JOINs (INNER JOIN between job_postings, companies, and company_industries to get company job postings).
- Aggregations (COUNT for job postings per company, AVG for size and job posting correlation).

### 4. Benefits Analysis for Data Science Jobs
- What benefits are most commonly offered in data science job postings?
- Is there a correlation between benefits offered and salary for data science roles?
- Which companies offer the most comprehensive benefits packages?

SQL Skills:
- JOINs (LEFT JOIN between benefits and job_postings to gather benefit information per job posting).
- Aggregations (COUNT, GROUP BY to calculate the frequency of each benefit).
- Subqueries (to compare salary with the number of benefits offered).

### 5. Job Market Distribution and Location Insights
- Where are the highest paying data science jobs located globally?
- How does the number of job postings vary across different cities or countries?
- Are there any geographical patterns in the industries offering data science jobs?

SQL Skills:
- JOINs (INNER JOIN between job_postings, companies, and company_industries to analyze job distribution).
- Window Functions (for ranking job locations based on salary).
- Aggregations (COUNT, SUM to track job posting counts by location).

### 6. Industry Growth and Forecasting
- Which industries are experiencing the fastest growth in data science job postings?
- Which industries feature the widest salary ranges for data science roles, and what factors influence these variations?
- What industries offer the most stable opportunities for data professionals?

SQL Skills:
- Window Functions (for ranking industries based on growth rate of job postings).
- CTEs (to handle and simplify complex time-series analysis).
- Aggregations (SUM, COUNT to track industry-specific trends).
---

## Advanced SQL Project: Data Science Job Market Analysis with Multiple JOINS

### 1. **Salary Trends and Insights**
   - What is the average salary for data science jobs across different industries?
   - Which companies offer the highest-paying data science roles?
   - How do salaries vary by location across all job postings?

   **SQL Skills:**
   - `INNER JOIN`, `AVG()`, `GROUP BY`, `ORDER BY`, `LEFT JOIN`

### 2. **Skill Demand and Growth**
   - Which skills are most in demand for data science roles globally?
   - What skills are associated with the highest-paying data science roles?
   - How has the demand for Python skills changed over the last 3 years?

   **SQL Skills:**
   - `LEFT JOIN`, `COUNT()`, `GROUP BY`, `AVG()`, `EXTRACT()`, `INNER JOIN`

### 3. **Company Overview and Job Postings Analysis**
   - Which companies post the most data science jobs?
   - How does the company size correlate with the number of job postings?
   - What industries are the most active in posting data science jobs?

   **SQL Skills:**
   - `LEFT JOIN`, `COUNT()`, `GROUP BY`, `INNER JOIN`, `ORDER BY`

### 4. **Benefits Analysis for Data Science Jobs**
   - What benefits are most commonly offered in data science job postings?
   - Is there a correlation between the number of benefits offered and salary?
   - Which companies offer the most comprehensive benefits packages?

   **SQL Skills:**
- `LEFT JOIN`, `COUNT()`, `AVG()`, `GROUP BY`, `INNER JOIN`
