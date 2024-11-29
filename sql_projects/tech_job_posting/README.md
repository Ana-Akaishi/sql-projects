![Alt text](https://images.unsplash.com/photo-1508780709619-79562169bc64?q=80&w=1740&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

# Tech Job Posting (TJP)
This project explores datasets related to data science job salaries, job postings, and required skills to analyze salary trends, skill demand, and industry opportunities. Using advanced SQL techniques, the project focuses on integrating data from multiple tables to uncover valuable insights into the global job market for data professionals.

I'm using free datasets on Kaggle:
- [Data Science Salaries 2020-2023](https://www.kaggle.com/datasets/arnabchaki/data-science-salaries-2023)
- [LinkedIn Job Postings Dataset](https://www.kaggle.com/datasets/rajatraj0502/linkedin-job-2023?select=company_specialities.csv)

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
### **1. Salary Analysis**  
- What is the average salary for data science roles across experience levels?
- Which job titles have the highest salaries, and how do they vary by company size?
- How do remote and on-site roles compare in salary ranges?

**SQL Skills:**  
- **INNER JOIN** to link job titles and company size.  
- **Aggregations** (`AVG`, `MAX`) for salary comparisons.  
- **Window Functions** to rank salaries by job title and experience level.

---

### **2. Regional Insights**  
- Which countries offer the highest salaries for data science jobs?
- How does an employee’s residence compare to the company’s location for remote roles?
- What is the proportion of fully remote roles by region?

**SQL Skills:**  
- **INNER JOIN** between `employee_residence` and `company_location` for regional analysis.  
- **LEFT JOIN** to include companies with incomplete remote data.  
- **CASE** to classify remote work levels (`0`, `50`, `100`).

---

### **3. Skill Demand Trends**  
- What are the top 10 most frequently required technical skills?
- Which industries demand specific skills like AI or cloud computing?  
- How does skill demand vary by company size? 

**SQL Skills:**  
- **INNER JOIN** between `job_postings.csv` and `job_skills.csv`.  
- **FULL OUTER JOIN** to compare skill demand across industries.  
- **CTEs** to extract and rank the most in-demand skills.

---

### **4. Benefits and Perks**  
- What are the most common benefits offered for remote roles? 
- Which company sizes are most likely to offer comprehensive perks?
- How do benefits vary across different industries?

**SQL Skills:**  
- **LEFT JOIN** between `benefits.csv` and `job_postings.csv` to analyze job perks.  
- **Aggregations** to calculate the prevalence of benefits by job type.  
- **Subqueries** to identify roles with multiple benefits.

---

### **5. Emerging Industries and Future Trends**
- Which industries are hiring the most data professionals?
- What percentage of companies in emerging industries offer remote opportunities?
- How do salaries vary across industries for data-related roles?

**SQL Skills:**  
- **INNER JOIN** between `job_postings.csv` and `company_industries.csv` for analyzing industry-specific hiring trends.  
- **LEFT JOIN** to include companies missing specific job postings.  
- **Aggregations** to compute averages and percentages across industries.  
- **Window Functions** to rank industries by the number of remote opportunities and average salaries.

---
