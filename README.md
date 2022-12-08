# Data modeling and ETL

### 1. Discuss the purpose of this database in the context of the startup, Sparkify, and their analytical goals.
This project serves the purpose for an imaginary startup company "Sparkify" to fetch user data and transfer to postgresql data base for future analysis

### 2. How to run the Python scripts
Run "create_tables.py" firstly then run "etl.py"  
### 3. An explanation of the files in the repository  
1. sql_queries.py  
Serves as an internal library for SQL querries to create/insert/select from tables in postgresql database
2. create_tables.py  
Serves as the main script to create fact and dimension tables in postgresql database 
3. etl.py  
Serves as the main ETL script to convert .json files in /data to postgresql database
### 4. State and justify your database schema design and ETL pipeline.
#### Database schema

#### ETL pipeline
### 5. [Optional] Provide example queries and results for song play analysis.
