# The_system_processes_and_analyzes_log_data_from_the_Online_Recruitment_Platform
This project focuses on building a system for processing and analyzing data from system logs. The main objective is to collect and process log data from various systems and applications, then store it in distributed databases like Cassandra (Data lake) for saving and MySQL for data warehousing.
Kafka for the messaging queue and put the raw data to Cassandra, PySpark for transforming the data from Cassandra then put the processed data to MySQL, MySQL for data warehousing, Airflow for scheduling the Python scripts. Using Docker to deploy the project easily.
- Tech stack: PySpark, Airflow, Kafka, Docker, Cassandra, MySQL.






## Pre-requisite
### Kafka setup
- Read "Run kafka sever.txt" in folder "kafka".
### Spark setup
- Install Spark (used 3.4.0)
### Airflow setup
- Install Airflow in Docker Compose
### Cassandra setup
- Install Cassandra
### MySQL setup
- Install MySQL
