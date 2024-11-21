![Alt text](https://github.com/Ana-Akaishi/sql-projects/blob/main/sql_project_banner.png)

# SQL
This repository will display some projects of how to use SQL to answer business questions. Companies usually use SQL to quick extract data. Once you write a query, the data will always come the same way, making it reliable for business routines or reports.

SQL is an easy language to understand, since the basics are close to what we do on daily basis. Think SQL as if you were writing how you look or open a file. If you write your steps I'm sure you'll find some similarities!

## Tech Tools
For display purposes, I'm going to use Jupyter notebook combined with `sqlite3`. 

`sqlite3` is a package that allows to write SQL queries in python. This way, I can write my comments step by step to you guys. And also, it's an interesting way to show how combine two different programing languages in one.

AS for my data, I'm going to use public data available on Kaggle. I'll link the databse in each project in case you want to check it out. Since I'm using kaggle data, the files will be in `.csv` format, but don't worry! We can use `pandas` to transform `.csv` to `sql`

Python, SQL

### How to install sqlite3
First install the package `ipython-sql` and `sqlite3`. Those will help us read csv files as if they were a database and use SQl within the notebook.

1. On your terminal you'll run
```
pip install ipython-sql sqlite3
```

2. Then call the pacakges in your notebook:
```
import pandas as pd
import sqlite3

# Load csv file
csv = pd.read_csv('kaggle_file.csv')

# Create a connection with SQLite
## Here I'm creating a temporary database using RAM
conn = sqlite3.connect(':memory:')

# Load pandas dataframe in SQL database format
csv.to_sql('table_name', conn, index = False, if_exists = 'replace')

# Load SQL language on Jupyter
%load_ext sql
%sql sqlite:///:memory:

# Make Jupyter accept SQL commands after %% using SQL Magic (from ipython-sql)
%config SqlMagic.conn = conn

# Now your notebook is ready to use SQL language!
# Keep in mind that all databases used in the notebook are temporary, changes won't be saved
# Also, since we are using our RAM memory to store this temporary data
# Make sure to use a light to medium dataset.

```

### Educational Resources
If you want to know more about SQL and how to learn it, check out my [SQL Study](https://github.com/Ana-Akaishi/sql-projects/tree/main/sql_study).

## SQL Projects
- [Brazilian Investment Funds Overview](https://github.com/Ana-Akaishi/data-science-projects/tree/main/Brazilian%20Investment%20Funds):  C