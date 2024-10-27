# Change-Data-Capture
**CDC with Debezium, Kafka, Postgres, Docker**

Overview
---
**Change data capture (CDC)** is a software design pattern that tracks and captures changes to data in a database and then delivers those changes to a downstream system in real-time. CDC is a method of Extract, Transform, Load (ETL) that can help organizations achieve data integrity and consistency across multiple systems. 

This Python script is designed to generate simulated financial transactions and insert them into a **PostgreSQL** database. It's particularly useful for setting up a test environment for Change Data Capture (CDC) with **Debezium**. The script uses the faker library to create realistic, yet fictitious, transaction data and inserts it into a PostgreSQL table.

System Architecture
---
![Architecture](https://github.com/user-attachments/assets/c8edc998-7b76-459b-9efc-5f41111d0c9e)

Prerequisites
---
Before running this script, ensure you have the following installed:

* Python 3.9+
* psycopg2 library for Python
* faker library for Python
* PostgreSQL server running locally or accessible remotely
* Docker and Docker Compose installed on your machine.
* Basic understanding of Docker, Kafka, and Postgres.

**Installation**
---
Install Required Python Libraries:
`pip install psycopg2-binary faker`

Services in the Compose File
---
* **Zookeeper**: A centralized service for maintaining configuration information, naming, providing distributed synchronization, and providing group services.
* **Kafka Broker**: A distributed streaming platform that is used here for handling real-time data feeds.
* **Confluent Control Center**: A web-based tool for managing and monitoring Apache Kafka.
* **Debezium**: An open-source distributed platform for change data capture.
* **Debezium UI**: A user interface for managing and monitoring Debezium connectors.
* **Postgres**: An open-source relational database.

  Commands
  ---
  **Run Docker Compose**: `docker-compose up -d` <br>
  **Verify the Services**: `docker-compose ps` <br>
  **Accessing the Services**: <br>
    * Kafka Control Center is accessible at `http://localhost:9021`. <br>
    * Debezium UI is accessible at `http://localhost:8080`. <br>
    * Postgres is accessible on the default port `5432`. <br> 
**Shutting Down**: `docker-compose down` <br>
