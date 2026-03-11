Since you are building a **Data Engineering GitHub repository**, after **Cassandra**, the next good topic is **Apache Kafka**.

---

# Apache Kafka (for GitHub Notes)

## File Name

`11_Apache_Kafka.md`

---

# Apache Kafka

## Definition

**Apache Kafka** is a **distributed event streaming platform** used for **real-time data streaming and data pipelines**.

Simple meaning:
Kafka is used to **send data from one system to another system in real time**.

Example:
Website → Kafka → Data Pipeline → Data Warehouse

---

## Why Kafka is Used

1. **Real-time data streaming**
2. **High throughput** (handles millions of messages)
3. **Scalable distributed system**
4. **Fault tolerant**
5. **Decouples systems** (producer and consumer independent)

---

## Core Components

### 1. Producer

System that **sends data to Kafka**.

Example:

* Application logs
* Website clicks
* IoT devices

---

### 2. Consumer

System that **reads data from Kafka**.

Example:

* Spark
* Data Warehouse
* Analytics system

---

### 3. Topic

A **category where messages are stored**.

Example:

```
topic: user_clicks
topic: payment_transactions
topic: logs
```

---

### 4. Broker

Kafka server that **stores and manages data**.

Kafka cluster can have **multiple brokers**.

---

### 5. Partition

Topic is divided into **partitions for scalability and parallel processing**.

Example:

```
Topic: Orders
Partition 1
Partition 2
Partition 3
```

---

## Kafka Architecture

```
Producer → Kafka Topic → Consumer
```

Example Data Pipeline:

```
Application
      ↓
Producer
      ↓
Kafka Topic
      ↓
Consumer
      ↓
Spark / Data Warehouse
```

---

## Real World Example

Example: **E-commerce website**

Events generated:

* User login
* Add to cart
* Payment
* Order placed

All events → **Kafka** → stored → processed by analytics system.

---

## Tools with Kafka

* **Apache Spark**
* **Apache Flink**
* **Apache Airflow**
* **Kafka Connect**
* **Kafka Streams**

---

## Interview Questions

### What is Kafka?

Kafka is a **distributed event streaming platform used for building real-time data pipelines and streaming applications**.

---

### Kafka vs Traditional Messaging System

| Feature        | Kafka     | Traditional MQ |
| -------------- | --------- | -------------- |
| Scalability    | High      | Medium         |
| Data Retention | Yes       | Limited        |
| Throughput     | Very High | Lower          |
| Distributed    | Yes       | Limited        |

---

### Kafka vs RabbitMQ

| Feature    | Kafka              | RabbitMQ      |
| ---------- | ------------------ | ------------- |
| Use Case   | Big Data Streaming | Message Queue |
| Throughput | Very High          | Medium        |
| Storage    | Persistent log     | Queue         |

---



```
01_Database_Fundamentals
02_Data_Types
03_Data_Processing
04_ETL_ELT
05_Data_Pipeline
06_Data_Warehouse
07_Data_Modeling
08_SQL_Basics
09_Data_Engineering_Tools
10_Apache_Cassandra
11_Apache_Kafka
12_Apache_Spark
13_Apache_Airflow
14_Data_Lake
15_Data Lakehouse
16_Stream Processing
17_Batch Processing
18_Data Governance
19_Data Quality
20_Data Security
```

