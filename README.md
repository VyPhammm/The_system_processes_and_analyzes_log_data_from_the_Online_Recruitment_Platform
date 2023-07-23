# The_system_processes_and_analyzes_log_data_from_the_Online_Recruitment_Platform
## Objective
This project focuses on building a data processing and analysis system from log data from users of a recruitment website. The main goal is to store, process, analyze that log data and decide the next step of the business development.
Kafka for the messaging queue and put the raw data to Cassandra (Data Lake), PySpark for transforming the data from Cassandra then put the processed data to MySQL, MySQL for data warehousing, Airflow for scheduling the Python scripts. Using Docker to deploy the project easily.
- Tech stack: PySpark, Airflow, Kafka, Docker, Cassandra, MySQL, Python.

## Architecture
  ![image](https://github.com/VyPhammm/The_system_processes_and_analyzes_log_data_from_the_Online_Recruitment_Platform/assets/127418764/bee618fb-cf02-4f61-a9ce-f156e78ef69c)

### Raw Data
- Log data schema
```sh
.
root
 |-- create_time: string (nullable = false)
 |-- bid: integer (nullable = true)
 |-- bn: string (nullable = true)
 |-- campaign_id: integer (nullable = true)
 |-- cd: integer (nullable = true)
 |-- custom_track: string (nullable = true)
 |-- de: string (nullable = true)
 |-- dl: string (nullable = true)
 |-- dt: string (nullable = true)
 |-- ed: string (nullable = true)
 |-- ev: integer (nullable = true)
 |-- group_id: integer (nullable = true)
 |-- id: string (nullable = true)
 |-- job_id: integer (nullable = true)
 |-- md: string (nullable = true)
 |-- publisher_id: integer (nullable = true)
 |-- rl: string (nullable = true)
 |-- sr: string (nullable = true)
 |-- ts: string (nullable = true)
 |-- tz: integer (nullable = true)
 |-- ua: string (nullable = true)
 |-- uid: string (nullable = true)
 |-- utm_campaign: string (nullable = true)
 |-- utm_content: string (nullable = true)
 |-- utm_medium: string (nullable = true)
 |-- utm_source: string (nullable = true)
 |-- utm_term: string (nullable = true)
 |-- v: integer (nullable = true)
 |-- vp: string (nullable = true)
```
<img width="1000" alt="image" src="https://github.com/VyPhammm/The_system_processes_and_analyzes_log_data_from_the_Online_Recruitment_Platform/assets/127418764/6d64c320-b765-462b-94fb-77954051faf8">

### Processing Data

### Clean data







## Setup
### Pre-requisite
#### Kafka setup
- Read "Run kafka sever.txt" in folder "kafka".
#### Spark setup
- Install Spark (used 3.4.0)
#### Airflow setup
- Install Airflow in Docker Compose
#### Cassandra setup
- Install Cassandra
#### MySQL setup
- Install MySQL
