# Change-Data-Capture
**CDC with Debezium, Kafka, Postgres, Docker**

Overview

**Change data capture (CDC)** is a software design pattern that tracks and captures changes to data in a database and then delivers those changes to a downstream system in real-time. CDC is a method of Extract, Transform, Load (ETL) that can help organizations achieve data integrity and consistency across multiple systems. 

This Python script is designed to generate simulated financial transactions and insert them into a **PostgreSQL** database. It's particularly useful for setting up a test environment for Change Data Capture (CDC) with **Debezium**. The script uses the faker library to create realistic, yet fictitious, transaction data and inserts it into a PostgreSQL table.

![Architecture](https://github.com/user-attachments/assets/c8edc998-7b76-459b-9efc-5f41111d0c9e)

Prerequisites
Before running this script, ensure you have the following installed:

Python 3.9+
psycopg2 library for Python
faker library for Python
PostgreSQL server running locally or accessible remotely
Docker and Docker Compose installed on your machine.
Basic understanding of Docker, Kafka, and Postgres.


