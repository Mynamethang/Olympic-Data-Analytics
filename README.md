# tokyo-olympic-azure-data-engineering-project

## Project Descrtiption:
In this project, I built a project that runs in Azure Cloud Service and perform the ETL process of Olympic Data dataset from kaggle.
<img src='project-idea.png' width=500>

## 1. Extraction

Create a workflow automation in Azure DataFactory to extract the data from kaggle and store in Data Lake Gen2 container automatically.

<img src='Extract-data-workflow.png' width=500>

There are 5 CSV datasets:
  - Athletes
  - Coaches
  - EntriesGender
  - Medals
  - Teams
<img src='Datalake-datasets.png' width=500>
## 2. Transformation

Deploy Databrick and utilize Pyspark to implement some basic data transformations such as formating datatype, sorting and cleaning. Then performing neccesary aggregations.

<img src='Performing-data-transformation.png' width=500>

After finishing transformation tasks, I restored transformed data onto Data Lake Gen2.

## 3. Loading

Using Azure Synapse Analytics to ingests transfomred data from Data Lake Gen2. Then Writing query to find insights of the data in Azure Synapase Lake database.

<img src='Query-in-Synapse-workspace.png' width=500>

# 4. Visualization

After gathering all analyzed data, I created dashboard that visualize the insights in PowerBI
