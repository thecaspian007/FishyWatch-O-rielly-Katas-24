# Data Fabric for Fishy Watch System

***Data Fabric*** is the software system responsible for managing data integration, transformation, storage, and access within the Fishy Watch system. It ensures data consistency, reliability, and scalability across heterogeneous data sources and analytical workflows.

## Component Details

| Component Name  | Component Description | Technology Choices |
| ------------- | ------------- | ------------- |
| ***Data Integration Layer***  | Integration layer for connecting and aggregating data from diverse sources such as sensors, databases, APIs, and external data providers. | MQTT Broker, RabbitMQ, Custom Data Ingestion Scripts |
| ***Data Processing Engine***  | Engine for batch and real-time data processing, transformation, enrichment, and cleansing to prepare data for analytics, machine learning, and reporting. | Pandas, NumPy, Scikit-Learn, Keras |
| ***Data Storage and Management***  | Storage solutions for structured and unstructured data, including data lakes, data warehouses, NoSQL databases, and object storage for scalable, high-performance data storage and retrieval. | Google Cloud Storage (GCS), PostgreSQL, Elasticsearch, Redis, BigQuery |
| ***Data Governance and Security***  | Governance framework for data access control, data lineage tracking, data quality monitoring, metadata management, and compliance with data privacy regulations. | Google Cloud Platform, Data Quality Tools, Encryption Tools |
| ***Data Access APIs***  | APIs and services layer for providing data access, query interfaces, data cataloging, and data virtualization capabilities to enable seamless data consumption by applications and users. | RESTful APIs, Elasticsearch, Metabase, Grafana, BigQuery |

### Component Diagram
![Data Fabric Component Diagram](../Assets/components/data-fabric.png)

## Architectural Characteristics

| Characteristics  | Decisions |
| ------------- | ------------- |
| Scalability  | Scalable architecture design to handle large volumes of data, concurrent users, and varied data processing workloads efficiently. |
| Reliability  | Implementation of fault-tolerant mechanisms, data replication, backup strategies, and disaster recovery plans to ensure data availability and durability. |
| Data Quality  | Integration of data quality checks, validation rules, anomaly detection, and data profiling techniques to maintain data accuracy, consistency, and reliability. |
| Performance  | Optimization of data processing pipelines, caching strategies, indexing techniques, and query optimization for fast data access and real-time analytics. |

## Architectural Choice

- Data Mesh Architecture for decentralized data ownership, domain-oriented data domains, and self-serve data capabilities aligned with Fishy Watch business domains.

## Deployment View
Below is the deployment view based on the architecture choice and this ADR [Deploy Data Fabric System in cloud.md](../ADRs/014-deployment-strategy.md)

![Data Fabric Deployment View](../Assets/deployment/data-fabric.png)
