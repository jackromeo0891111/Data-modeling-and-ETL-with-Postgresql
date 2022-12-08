# Data modeling and ETL
This project serves the purpose for an imaginary startup company "Sparkify" to fetch user data and transfer to postgresql database for future analysis

### 1. How to run the Python scripts?
Run "create_tables.py" firstly then run "etl.py"  
### 2. An explanation of the files in the repository  
**1. sql_queries.py**  
Serves as an internal library for SQL querries to create/insert/select from tables in postgresql database  
**2. create_tables.py**  
Serves as the main script to create fact and dimension tables in postgresql database  
**3. etl.py**  
Serves as the main ETL script to convert .json files in /data to postgresql database  
### 3. Database schema design and ETL pipeline
#### Database Schema  
![database schema](https://user-images.githubusercontent.com/88352138/206338270-96bdc149-56ae-469b-bb7a-ae430e1bada9.JPG)  
#### ETL pipeline
![ETL pipeline](https://user-images.githubusercontent.com/88352138/206355922-da802f16-0dcf-4de6-8dd4-27a688a7f78d.JPG)

### 4. example queries and results  
```sql
SELECT * FROM songplays LIMIT 5;
```
|songplay_id|	start_time|	user_id|	level|	song_id|	artist_id|	session_id|	location|	user_agent|
|-----------|-----------|--------|-------|---------|-----------|------------|---------|-----------|
|0	|2018-11-30 00:22:07.796000|	91|	free|	SOMZWCG12A8C13C480|	ARD7TVE1187B99BFB1|	829|	Dallas-Fort Worth-Arlington, TX|	Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.2; WOW64; Trident/6.0)|
|1|	2018-11-30 01:08:41.796000|	73|	paid|	SOMZWCG12A8C13C480|	ARD7TVE1187B99BFB1|	1049|	Tampa-St. Petersburg-Clearwater, FL|	"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_4) AppleWebKit/537.78.2 (KHTML, like Gecko) Version/7.0.6 Safari/537.78.2"|
|2|	2018-11-30 01:12:48.796000|	73|	paid|	SOMZWCG12A8C13C480|	ARD7TVE1187B99BFB1|	1049|	Tampa-St. Petersburg-Clearwater, FL|	"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_4) AppleWebKit/537.78.2 (KHTML, like Gecko) Version/7.0.6 Safari/537.78.2"|
|3|	2018-11-30 01:17:05.796000|	73|	paid|	SOMZWCG12A8C13C480|	ARD7TVE1187B99BFB1|	1049|	Tampa-St. Petersburg-Clearwater, FL|	"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_4) AppleWebKit/537.78.2 (KHTML, like Gecko) Version/7.0.6 Safari/537.78.2"|
|4|	2018-11-30 01:20:56.796000|	73|	paid|	SOMZWCG12A8C13C480|	ARD7TVE1187B99BFB1|	1049|	Tampa-St. Petersburg-Clearwater, FL|	"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_4) AppleWebKit/537.78.2 (KHTML, like Gecko) Version/7.0.6 Safari/537.78.2"|
