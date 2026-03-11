Next topic for your **Data Engineering GitHub repository**:

# Apache Airflow

## File Name

`13_Apache_Airflow.md`

---

# Apache Airflow

## Definition

**Apache Airflow** is an **open-source workflow orchestration tool** used to **schedule, manage, and monitor data pipelines**.

Simple meaning:
Airflow helps **automatically run data pipelines in the correct order**.

Example:

```text
Extract Data → Transform Data → Load to Data Warehouse
```

Airflow makes sure each step runs **at the right time and in the right sequence**.

---

# Why Airflow is Used

1. **Automates data pipelines**
2. **Schedules tasks**
3. **Manages workflow dependencies**
4. **Monitors pipeline status**
5. **Handles retries if tasks fail**

Example:
Daily pipeline:

```text
1 AM → Extract data  
2 AM → Transform data  
3 AM → Load to warehouse
```

Airflow runs this **automatically**.

---

# Core Components

## 1. DAG (Directed Acyclic Graph)

A **workflow definition** that defines tasks and their order.

Example:

```text
Extract → Transform → Load
```

---

## 2. Task

A **single unit of work** inside a pipeline.

Example tasks:

* Extract data
* Clean data
* Load data

---

## 3. Operator

Operator defines **what the task should do**.

Examples:

* PythonOperator
* BashOperator
* EmailOperator
* SQL Operator

---

## 4. Scheduler

The **scheduler triggers pipelines** based on time or events.

Example:

* Every day
* Every hour

---

## 5. Web UI

Airflow provides a **web interface** to:

* Monitor pipelines
* View logs
* Debug failures

---

# Airflow Architecture

```text
DAG
 ↓
Scheduler
 ↓
Workers
 ↓
Tasks Execution
 ↓
Metadata Database
```

---

# Example Data Engineering Pipeline

```text
Data Source
      ↓
Airflow DAG
      ↓
Extract Data
      ↓
Transform Data (Spark / Python)
      ↓
Load Data (Data Warehouse)
```

---

# Example Airflow DAG

```python
from airflow import DAG
from airflow.operators.bash import BashOperator
from datetime import datetime

dag = DAG('example_pipeline', start_date=datetime(2024,1,1))

task1 = BashOperator(
    task_id='extract_data',
    bash_command='echo Extracting data',
    dag=dag
)
```

---

# Airflow vs Cron

| Feature             | Airflow | Cron |
| ------------------- | ------- | ---- |
| Workflow management | Yes     | No   |
| Task dependency     | Yes     | No   |
| Monitoring          | Yes     | No   |
| Scheduling          | Yes     | Yes  |

---

# Companies Using Airflow

* Airbnb
* Netflix
* Spotify
* LinkedIn

