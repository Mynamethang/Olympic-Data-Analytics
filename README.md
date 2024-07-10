# tokyo-olympic-azure-data-engineering-project

## Project Descrtiption:
In this project, I built a project that runs in Azure Cloud Service and perform the ETL process of Olympic Data dataset from kaggle.

![azure drawio](https://github.com/Mynamethang/Olympic-Data-Analytics/assets/109019819/b7819c9d-50e6-4c4e-ad2f-c1251e1128c8)


## 1. Extraction

Create a workflow automation in Azure DataFactory to extract the data from kaggle and store in Data Lake Gen2 container automatically.

<img src='Extract-data-workflow.png' width=700>

There are 5 CSV datasets:
  - Athletes
  - Coaches
  - EntriesGender
  - Medals
  - Teams
<img src='Datalake-datasets.png' width=700>
## 2. Transformation

Deploy Databrick and utilize Pyspark to implement some basic data transformations such as formating datatype, sorting and cleaning. Then performing neccesary aggregations.

<img src='Performing-data-transformation.png' width=700>

After finishing transformation tasks, I restored transformed data onto Data Lake Gen2.

## 3. Loading

Using Azure Synapse Analytics to ingests transfomred data from Data Lake Gen2. Then Writing query to find insights of the data in Azure Synapase Lake database.

<img src='Query-in-Synapse-workspace.png' width=700>

# 4. Visualization

After gathering all analyzed data, I created dashboard that visualize the insights in PowerBI
