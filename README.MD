# 🚦 Smart City Mobility Insights – ELT Portfolio Project

## 🧠 Overview
This project simulates a real-world ELT pipeline designed to help city planners optimize public transportation using data from multiple sources. It demonstrates my ability to build scalable, testable, and insightful data workflows using modern tools.

## 📊 Use Case
A European city wants to improve mobility by analyzing:
- Bus GPS data
- Bike-sharing usage
- Weather conditions
- Citizen feedback (sentiment analysis)

## 🏗️ Architecture
The pipeline follows a modular ELT approach:
1. **Extract & Load**: Airbyte pulls data from APIs and flat files into PostgreSQL staging.
2. **Transform**: dbt Core models clean and enrich the data.
3. **Warehouse**: Final models are stored in PostgreSQL.
4. **Quality**: Great Expectations validates data integrity.
5. **Orchestration**: Prefect schedules and monitors the pipeline.
6. **Visualization**: Tableau dashboards provide actionable insights.
7. **Notification**: Slack alerts notify stakeholders of pipeline status.

The data sources are multi-cloud and hybrid in nature:
- MySQL (operational data)
- AWS S3 (data lake storage)
- AWS Redshift (warehouse)
- Google Cloud Storage (feedback archive)

## 🧰 Tech Stack
| Stage           | Tool                 |
|-----------------|----------------------|
| Generate        | Python (JupyterLab)  |
| Extract & Load  | Airbyte              |
| Staging         | DuckDB               |
| Transform       | dbt Core             |
| Warehouse       | PostgreSQL           |
| Quality         | Great Expectations   |
| Orchestrate     | Prefect              |
| Visualize       | Tableau              |
| Notify          | Slack / Email        |

## 📦 Folder Structure
smart-city-elts/
├── 00 synthetic data/  
├── 01 airbyte/ 
├── 02 dbt/ 
├── 03 prefect/ 
├── 04 expectations/ 
├── 05 dashboards/ 
├── 06 docs/ 
└── README.md

## 🚀 How to Run
1. Clone the repo
2. Set up Airbyte connectors
3. Run dbt models
4. Launch Prefect flows
5. View dashboards in Tableau

## ✅ Data Quality
Implemented tests for:
- Null values
- Schema drift
- Outliers in ridership

## 📈 Dashboards
- Peak Hour Analysis
- Weather vs Ridership
- Sentiment Trends

## 🧠 Lessons Learned
- Importance of modular transformations
- Handling schema evolution in real-time feeds
- Balancing performance vs cost in orchestration

## 📬 Contact
Feel free to reach out via [your email] or [your website] for feedback or collaboration!
