Next topic for your **Data Engineering GitHub repository**:

# Apache Spark

## File Name

`12_Apache_Spark.md`

---

# Apache Spark

## Definition

**Apache Spark** is an **open-source distributed data processing engine** used for **large-scale data processing and analytics**.

Simple meaning:
Spark is used to **process very large amounts of data quickly across multiple machines**.

Example:
Logs → Spark → Process → Data Warehouse

---

# Why Spark is Used

1. **Fast processing** (in-memory computation)
2. **Handles big data**
3. **Distributed processing**
4. **Supports multiple languages**
5. **Works with batch and streaming data**

---

# Spark Core Components

## 1. Spark Core

The **main engine** responsible for:

* Memory management
* Task scheduling
* Distributed processing

---

## 2. Spark SQL

Used for **structured data processing using SQL queries**.

Example:

```sql
SELECT * FROM users WHERE country = 'India';
```

---

## 3. Spark Streaming

Used to **process real-time streaming data**.

Example:

* Kafka data stream
* IoT data
* Website events

---

## 4. MLlib

Machine Learning library in Spark.

Used for:

* Classification
* Regression
* Clustering
* Recommendation systems

---

## 5. GraphX

Used for **graph processing**.

Example:

* Social networks
* Relationship graphs

---

# Spark Architecture

```text
Driver Program
      ↓
Cluster Manager
      ↓
Worker Nodes
      ↓
Executors
      ↓
Tasks
```

---

# Important Spark Concepts

## RDD (Resilient Distributed Dataset)

A **distributed collection of data** that can be processed in parallel.

---

## DataFrame

A **structured table format** like SQL tables.

Example:

| id | name | country |
| -- | ---- | ------- |
| 1  | Arun | India   |

---

## Dataset

A **type-safe distributed data structure**.

---

# Spark vs Hadoop MapReduce

| Feature     | Spark     | Hadoop MapReduce |
| ----------- | --------- | ---------------- |
| Speed       | Very Fast | Slow             |
| Processing  | In-memory | Disk-based       |
| Real-time   | Yes       | No               |
| Ease of Use | Easy      | Complex          |

---

# Spark in Data Engineering Pipeline

Example pipeline:

```text
Data Source
      ↓
Kafka
      ↓
Spark Processing
      ↓
Data Warehouse
      ↓
BI Tools
```

---

# Tools Used With Spark

* Apache Kafka
* Hadoop
* AWS S3
* Apache Airflow
* Delta Lake

---

# Real World Companies Using Spark

* Netflix
* Uber
* Amazon
* Facebook

