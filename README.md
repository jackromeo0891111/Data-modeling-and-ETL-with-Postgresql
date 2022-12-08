# Data modeling and ETL
This project serves the purpose for an imaginary startup company "Sparkify" to fetch user data and transfer to postgresql data base for future analysis

### 1. How to run the Python scripts
Run "create_tables.py" firstly then run "etl.py"  
### 2. An explanation of the files in the repository  
**1. sql_queries.py**  
Serves as an internal library for SQL querries to create/insert/select from tables in postgresql database  
**2. create_tables.py**  
Serves as the main script to create fact and dimension tables in postgresql database  
**3. etl.py**  
Serves as the main ETL script to convert .json files in /data to postgresql database  
### 3. State and justify your database schema design and ETL pipeline.
#### Database schema
![database schema](https://user-images.githubusercontent.com/88352138/206338270-96bdc149-56ae-469b-bb7a-ae430e1bada9.JPG)
#### ETL pipeline
### 5. [Optional] Provide example queries and results for song play analysis.
