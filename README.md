# Traffic Monitor Server (tm-server)

This repo will store the server-side code and deployments for collecting and serving data for the Traffic Monitor.

## Features and stack
* Database storage - Apache Druid will be used for long-term, comprehensive storage for all Traffic Monitor collected data
* Data Visualiztion (Business Intelligence)- Apache Superset will be used to analyze databases
* Data Governance - Apache Atlas will be used to catalog and capture metadata round data and transformations

## Installation

### Superset
Apache Superset Docker containers need to be built from [superset GitHub source](https://github.com/apache/superset).  Instructions can be found at [Superset quickstart](https://superset.apache.org/docs/quickstart/).

### Druid
[Apache Druid](https://github.com/apache/druid) Docker can be deployed from the Docker compose scripts under `distribution/docker`.  Instructions can be found on [Druid Run with Docker](https://druid.apache.org/docs/latest/tutorials/docker/).

### Airflow
Apache Airflow Docker containers can be depoloyed from Docker compose scripts. Instructions can be found on [Running Airflow in Docker](https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html).

### ThingsBoard.io (CE)
[ThingsBoard](https://github.com/thingsboard/thingsboard) is an open-source IoT platform for data collection, processing, visualization, and device management. Instructions can be found on [Installing ThingsBoard using Docker](https://thingsboard.io/docs/user-guide/install/docker/).