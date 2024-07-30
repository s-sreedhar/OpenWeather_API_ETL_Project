# Automated ETL Pipeline Using Airflow on AWS EC2

## Overview
This project demonstrates how to build an automated ETL (Extract, Transform, Load) pipeline using Apache Airflow on an AWS EC2 instance. The pipeline connects to the OpenWeatherMap API to extract weather data, transforms the data, and loads it into an S3 bucket.

## Highlights
* 🌐 API Connection: Establish a connection to the OpenWeatherMap API using an HTTP sensor.
* 🔗 HTTP Connection Setup: Configure Airflow's HTTP connection for seamless API access.
* ⏳ API Readiness: Ensure the API is ready before extracting data to prevent downstream failures.
* 📊 Data Extraction: Extract weather data using a Python operator.
* ☁️ Data Loading: Load the transformed data into an S3 bucket.
* 🔑 Permission Management: Resolve AWS CLI permission issues.
* ✔️ Verification: Verify the successful storage of data in S3.

## Getting Started
### Prerequisites
- AWS account with necessary permissions.
- OpenWeatherMap API key.
- Basic knowledge of Airflow and AWS services.
### Steps
- Set Up AWS EC2 Instance
- Launch an EC2 instance and configure it for running Airflow.

  ### Install Airflow

- Install Apache Airflow on your EC2 instance.
  ### Configure OpenWeatherMap API
- Sign up for the OpenWeatherMap API and obtain an API key.
- Configure Airflow’s HTTP connection with the API key.

 ### Create the Airflow DAG
- Define an Airflow DAG (Directed Acyclic Graph) to schedule and manage the ETL tasks.

 ### Extract Data
- Use a Python operator to connect to the OpenWeatherMap API and extract weather data.

  ### Transform Data
- Process and transform the extracted data to ensure it is in the desired format.

### Load Data
- Store the transformed data in an AWS S3 bucket.

### Resolve Permissions
- Configure the AWS CLI and resolve any IAM role or access key issues to ensure proper permissions.

 ### Verify Data Storage
- Check the S3 bucket to ensure that the data has been successfully loaded.
