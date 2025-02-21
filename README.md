## 📌 **The GOAL**
This project aims to collect, transform, and visualize real-time sensor data using **Snowflake** and **Power BI**, with a flexible pipeline that can evolve into a more robust solution over time.

## 🏗️ **Tech Stack**
- **Ingestion**: JSON/CSV files sent to cloud storage (S3/Azure Blob) via **Snowpipe** for near real-time ingestion.
- **Storage**: **Snowflake** (staging tables, transformed tables for analytics, real-time data handling).
- **Transformation**: **SQL** in Snowflake (views, stored procedures).
- **Automation**: **Snowflake Streams & Tasks** to automate the processing of new data.
- **Visualization**: **Power BI** with **DirectQuery** to display real-time data.
- **Version Control**: **Git** with **GitHub** (to version all code, SQL, ingestion scripts).

  **Future Improvements**:
  - Transition to streaming solutions like **Kafka** or **MQTT**.
  - Add **dbt** to manage more complex transformations.
  - Integrate **Airflow** or **Prefect** for advanced orchestration.
  - Add **Kubernetes** for container management and orchestration.

## 📂 **Repo Structure**
```
📦 MonProjetData
 ┣ 📂 docs
 ┃ ┗ 📄 architecture.md  # Architecture diagram detailing the data flow
 ┣ 📂 src
 ┃ ┗ 📄 ingestion.py  # Data ingestion script from Cloud Storage
 ┣ 📂 sql
 ┃ ┗ 📄 create_tables.sql  # SQL script to create tables in Snowflake
 ┣ 📂 terraform          # Scripts for managing infrastructure (future)
 ┣ 📄 .gitignore
 ┣ 📄 README.md  # Project explanation and getting started guide
```
