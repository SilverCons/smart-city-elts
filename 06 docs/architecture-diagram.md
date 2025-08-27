+------------------+       +------------------+       +------------------+
|  Data Sources    | --->  |    Airbyte       | --->  |   PostgreSQL     |
| (APIs, CSVs, IoT)|       | (Extract & Load) |       |   (Staging DB)   |
+------------------+       +------------------+       +------------------+
                                                           |
                                                           v
                                                  +------------------+
                                                  |     dbt Core     |
                                                  | (Transformations)|
                                                  +------------------+
                                                           |
                                                           v
                                                  +------------------+
                                                  |   PostgreSQL DW  |
                                                  | (Final Models)   |
                                                  +------------------+
                                                           |
                                                           v
                                                  +------------------+
                                                  |   Great Expectations |
                                                  | (Data Quality Checks)|
                                                  +------------------+
                                                           |
                                                           v
                                                  +------------------+
                                                  |     Prefect      |
                                                  | (Orchestration)  |
                                                  +------------------+
                                                           |
                                                           v
                                                  +------------------+
                                                  |     Tableau      |
                                                  | (Visualization)  |
                                                  +------------------+
                                                           |
                                                           v
                                                  +------------------+
                                                  | Notifications    |
                                                  | (Slack / Email)  |
                                                  +------------------+
