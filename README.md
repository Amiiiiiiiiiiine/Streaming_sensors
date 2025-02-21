## 📌 **The GOAL**
This project aims to collect, transform, and visualize real-time sensor data using **Snowflake** and **Power BI**, with a flexible pipeline that can evolve into a more robust solution over time.

## 🏗️ **Tech Stack**
| **Catégorie**        | **Choix Simple (V1)**                    | **Amélioration Future (V2+)** |
| -------------------- | ---------------------------------------- | ----------------------------- |
| **Version Control**  | Git + GitHub / GitLab                    | GitHub Actions (CI/CD)        |
| **Ingestion**        | Fichiers JSON/CSV chargés via Snowpipe   | Kafka / MQTT (streaming)      |
| **Stockage**         | Tables Snowflake (staging + transformée) | Data Vault / Time Travel      |
| **Transformation**   | SQL (views, stored procedures)           | dbt (Data Build Tool)         |
| **Orchestration**    | Snowflake Streams & Tasks                | Apache Airflow / Prefect      |
| **Automatisation**   | Manuelle via scripts                     | Terraform (Infra as Code)     |
| **Conteneurisation** | Docker pour les scripts d'ingestion      | Kubernetes (orchestration)    |
| **Visualisation**    | Power BI (DirectQuery)                   | Streamlit / Looker / Tableau  |
| **Monitoring**       | Snowflake Query Logging                  | Grafana / Datadog / ELK Stack |
| **Déploiement**      | Manuellement avec Git                    | Automatisation via CI/CD      |
| **Infrastructure**   | Snowflake & S3                           | Kubernetes (GKE, AKS, EKS)    |

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
