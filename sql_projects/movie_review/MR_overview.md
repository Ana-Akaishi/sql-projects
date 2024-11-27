# Movie Review (MR)
This projectt will dive into the entertainment industry! I'm going to use this [movies](https://developer.imdb.com/non-commercial-datasets/) databases by IMDb. This is an interesting project because I'll be using different databases, each one containing a different type of information about the movie and may contain null values.

## Objectives
The objective of this project is to deal with multiple databases and missing values:
- How to identify and treat missing values?
- Join tables
- Subqueries and aggregation functions
- Date manipulation

## Business Questions
### 1. Genre Popularity Analysis
- What are the top 5 most popular genres based on the number of films released?
- How does the average movie rating vary by genre?
- Which genres saw the biggest increase in the number of releases over the last 5 years?

SQL Skills:
- Joins (linking title.basics with genre-related tables).
- Aggregation functions (`COUNT()`, `AVG()`).
- Subqueries (for filtering by recent years).
- Sorting (`ORDER BY`).

### 2. Director Productivity Analysis
- Who are the directors with the most films in the catalog?
- What is the average rating for movies directed by each of the top 10 directors?
- Which director worked across the most genres?

SQL Skills:
- Joins (linking title.crew with title.basics).
- Aggregation functions (`COUNT()`, `AVG()`).
- Subqueries (to rank directors by number of movies).
- Grouping and filtering (`GROUP BY`, `HAVING`).

### 3. Yearly Production Trends
- Which year had the most film releases in total?
- What is the trend of movie releases over the last 10 years?
- How many movies and TV series were released in the same year?

SQL Skills:
- Date manipulation (using startYear and endYear).
- Aggregation functions (`COUNT()`).
- Subqueries (for year-over-year comparisons).
- Sorting and filtering (`GROUP BY`).

### 4. Movie Rating Trends
- What are the top 5 highest-rated movies?
- Which genre has the highest average movie rating?
- Is there a correlation between movie runtime and average rating?

SQL Skills:
- Joins (linking title.basics and title.ratings).
- Aggregation functions (`AVG()`, `MAX()`).
- Subqueries (for filtering by ratings).
- Sorting (`ORDER BY`).

### 5. TV Series and Movie Comparison
- What is the average rating of TV series compared to movies?
- Which TV series has the longest runtime and how does it compare to movies of similar genres?
- What percentage of releases in the last 5 years were TV series?

SQL Skills:
- Joins (linking title.basics, title.episode).
- Aggregation functions (`AVG()`, `COUNT()`).
- Date manipulation (using startYear and endYear).
- Sorting (`ORDER BY`) and filtering (`HAVING`).
