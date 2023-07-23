## Setup Airflow
 We will setup airflow on docker
- Clone git repo

``` git clone https://github.com/VyPhammm/The_system_processes_and_analyzes_log_data_from_the_Online_Recruitment_Platform &&  cd airflow``` 

- install docker
```docker-compose up```
- Visit: http://localhost:8080

### DAGs
DAG Flow 
- Compare data on Data Lake: Cassandra and data on Data WareHouse: MySQL, check whether new data is recorded on Cassandra or not? If no new data is available, print the message and stop running.
- If there is new data, then process the data ETL - Spark job.
- Storage data to Data Warehouse: MySQL.

