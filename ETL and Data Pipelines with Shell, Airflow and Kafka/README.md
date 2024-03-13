# Scenario

You are a data engineer at a data analytics consulting company. You have been assigned to a project that aims to de-congest the national highways by analyzing the road traffic data from different toll plazas. Each highway is operated by a different toll operator with different IT setup that use different file formats.  In the first Hands-on lab your job is to collect data available in different formats and, consolidate it into a single file.  

As a vehicle passes a toll plaza, the vehicle's data like vehicle_id,vehicle_type,toll_plaza_id and timestamp are streamed to Kafka. In the second Hands-on lab your job is to create a data pipe line that collects the streaming data and loads it into a database.

## Tasks and Solutions
- Task 1.1: Define DAG arguments \
![alt text]( https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/dag_args.png)
- Task 1.2: Define the DAG \
![alt text]( https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/dag_definition.png "dag_definition")
- Task 1.3: Create a task to download data \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/unzip_data.png "unzip_data")
- Task 1.4: Create a task to extract data from csv file \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/extract_data_from_csv.png "extract_data_from_csv")
- Task 1.5: Create a task to extract data from tsv file \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/extract_data_from_tsv.png "extract_data_from_tsv")
- Task 1.6: Create a task to extract data from fixed width file \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/extract_data_from_fixed_width.png "extract_data_from_fixed_width")
- Task 1.7: Create a task to consolidate data extracted from previous tasks \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/consolidate_data.png "consolidate_data")
- Task 1.8: Transform the data \
For this task, we can use the SELECT function to query the size of the database from information_schema.tables or using the show table status\
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/transform.png "transform")
- Task 1.9: Define the task pipeline \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/task_pipeline.png "task_pipeline")
- Task 1.10: Submit the DAG \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/submit_dag.png "submit_dag")
- Task 1.11: Unpause the DAG \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/unpause_dag.png "unpause_dag")
- Task 1.12: Monitor the DAG \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/dag_runs.png "monitor_dag")
- Task 2.1: Start Zookeeper \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/start_zookeeper.png "start_zookeeper")
- Task 2.2: Start Kafka server \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/start_kafka.png "start_kafka")
- Task 2.3: Create a topic named toll \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/create_toll_topic.png "create_toll_topic")
- Task 2.4: Download the Toll Traffic Simulator \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/download_simulator.png "download_simulator")
- Task 2.5: Configure the Toll Traffic Simulator \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/configure_simulator.png "configure_simulator")
- Task 2.6: Run the Toll Traffic Simulator \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/simulator_output.png "simulator_output")
- Task 2.7: Configure streaming_data_reader.py \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/streaming_reader_code.png "streaming_reader_code")
- Task 2.8: Run streaming_data_reader.py \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/data_reader_output.PNG "data_reader_output")
- Task 2.9: Health check of the streaming data pipeline \
![alt text](https://github.com/SandraMoses/IBM_BI-Foundations-with-SQL-ETL-and-Data-Warehousing-Specialization/blob/main/ETL%20and%20Data%20Pipelines%20with%20Shell%2C%20Airflow%20and%20Kafka/Final%20Assignment/output_rows.png "output_rows")
