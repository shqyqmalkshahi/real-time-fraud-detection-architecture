# real-time-fraud-detection-architecture
Designed a scalable real-time fraud detection architecture using big data technologies (NiFi, Kafka, Spark, HDFS, Hive, HBase) to support AML compliance and high-volume transaction monitoring.

# Real-Time Fraud Detection & AML Compliance Architecture

## Overview
This project presents a scalable big data architecture designed for real-time fraud detection and anti-money laundering (AML) compliance in financial systems. The architecture focuses on processing high-volume transaction streams, detecting anomalies in real time, and supporting regulatory reporting requirements.

---

## Problem Statement
Financial institutions process millions of transactions daily and must detect fraudulent behavior instantly to prevent financial loss. At the same time, they must comply with strict AML regulations, which require accurate monitoring, reporting, and traceability of suspicious activities.

Traditional batch processing systems are insufficient for these requirements, making real-time streaming architectures essential.

---

## Objective
To design a scalable, fault-tolerant system capable of:
- Processing real-time transaction data streams  
- Detecting anomalies and suspicious patterns  
- Generating risk scores for transactions  
- Supporting compliance reporting and investigations  

---

## Architecture Overview

The system is designed as a distributed big data pipeline with multiple integrated components:

### Data Ingestion
- **Apache NiFi** → Handles data ingestion from multiple sources (transaction systems, APIs)

### Streaming Layer
- **Apache Kafka** → Enables real-time data streaming and event processing

### Processing Layer
- **Apache Spark (Streaming)** → Performs real-time fraud detection, anomaly detection, and risk scoring

### Storage Layer
- **HDFS** → Distributed storage for large-scale transaction data  
- **HBase** → Low-latency access for real-time queries  

### Query & Reporting
- **Hive** → SQL-based querying and compliance reporting  

### Search & Investigation
- **Apache Solr** → Enables fast search for fraud investigation and auditing  

### Resource Management
- **YARN** → Manages cluster resources and workload distribution  

---

## System Workflow

1. Transaction data is ingested through NiFi  
2. Data is streamed into Kafka topics  
3. Spark processes the stream in real time  
4. Fraud detection logic assigns risk scores to transactions  
5. Data is stored in HDFS and indexed in HBase  
6. Hive enables reporting for compliance teams  
7. Solr supports investigation and search queries  

---

## Key Features

- Real-time fraud detection using streaming data  
- Scalable architecture for high transaction volumes  
- Fault-tolerant distributed system design  
- Integration of multiple big data technologies  
- Support for regulatory compliance and auditing  

---

## Business Value

- Reduces financial loss through early fraud detection  
- Enables compliance with AML regulations  
- Supports real-time monitoring of transactions  
- Improves investigation speed and accuracy  
- Scales efficiently with increasing data volume  

---

## Use Case

This architecture can be applied in:
- Banking transaction monitoring systems  
- Credit card fraud detection  
- Payment processing platforms  
- AML compliance systems  

---

## Limitations

- Requires complex infrastructure setup  
- High operational and maintenance costs  
- Requires tuning of fraud detection models  
- Dependent on data quality and latency  

---

## Future Improvements

- Integrate machine learning models for adaptive fraud detection  
- Add real-time alerting system for suspicious transactions  
- Incorporate user behavior analytics  
- Optimize latency for ultra-low response times  

---

## Project Structure

- `.pptx` → architecture design presentation  
- 🎥 Video presentation → explanation of system design  

---

## 🎥 Project Presentation
Watch the full video here:  
https://drive.google.com/file/d/1AnBc-QT6RcSO3voQYvrGHaok2zjLxln5/view?usp=sharing  

---

## Author
Shaghayegh Malekshahi  
Master’s in Data Science  
