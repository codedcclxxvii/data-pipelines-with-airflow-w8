# Data Pipelines with Airflow

## Background Information

Our telecommunications company, MTN Rwanda, has a vast customer base, and we generate a large amount of data daily. We must efficiently process and store this data to make informed business decisions. Therefore, we plan to develop a data pipeline to extract, transform, and load data from three CSV files and store it in a Postgres database. We require a skilled data engineer who can use the Airflow tool to develop the pipeline to achieve this.
Problem Statement
The main challenge is that the data generated is in a raw format, and we need to process it efficiently to make it usable for analysis. This requires us to develop a data pipeline that can extract, transform and load the data from multiple CSV files into a single database, which can be used for further analysis.

### Guidelines
The data pipeline should be developed using Airflow, an open-source tool for creating and managing data pipelines. The following steps should be followed to develop the data pipeline:

● The data engineer should start by creating a DAG (Directed Acyclic Graph) that defines the workflow of the data pipeline.

● The DAG should include tasks that extract data from the three CSV files.

● After extraction, the data should be transformed using Python libraries to match the
required format.

● Finally, the transformed data should be loaded into a Postgres database.

● The data pipeline should be scheduled to run at a specific time daily using the Airflow
scheduler.

● We can use the shared file (mtnrwanda-dag.py) as a starting point.

### Sample CSV Files

The following are sample CSV files that will be used in the data pipeline: 

● customer_data.csv

● order_data.csv

● payment_data.csv

All files for this project can be downloaded from here (link).
 
### Deliverables
We will be expected to deliver a GitHub repository with the following:

● Airflow DAG file for the data pipeline. - in this repo

● Documentation of the pipeline.

○ Highlight at least 3 best practices used during the implementation.
○ Recommendations for deployment and running the pipeline in a cloud-based
provider.

## Documentation

Developing a data pipeline using Airflow to extract, transform, and load data from CSV files into a mongodb database can be done using the following steps:

### Step 1: Setting up the Environment

Before creating the DAG, you need to set up the environment to run the pipeline. You need to install Apache Airflow, mongodb, and the required Python libraries for data processing.

### Step 2: Creating the DAG

The next step is to create the DAG that defines the workflow of the data pipeline. In Airflow, a DAG is a collection of tasks that are arranged in a specific order. Each task in a DAG represents a unit of work that needs to be executed.

The DAG should be created in a Python file and stored in the dags folder of the Airflow installation directory.

### Step 3: Defining Python Functions for Tasks

The next step is to define Python functions for each task in the DAG. These functions should contain the logic to extract, transform, and load data from the CSV files to the mongo database

## Deployment Recommendations:
<ul><li>
Use a cloud-based provider such as AWS, Azure or GCP to deploy the data pipeline. This makes it easier to scale the data pipeline as the amount of data grows.
</li>
<li>
Use a containerization technology such as Docker to package the data pipeline code and dependencies. This makes it easier to deploy the data pipeline to different environments.
</li>
<li>
Use an Infrastructure as Code (IaC) tool such as Terraform to provision the infrastructure needed for the data pipeline. This makes it easier to automate the deployment and ensure consistency across different environments.</li></ul>
