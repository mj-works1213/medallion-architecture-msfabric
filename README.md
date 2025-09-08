# Medallion Architecture Implementation in Microsoft Fabric
This project demonstrates a complete Medallion Architecture (Bronze → Silver → Gold) built using Microsoft Fabric pipelines and notebooks, showcasing how raw data is ingested, cleansed, transformed, and prepared for business-ready analytics.

# Bronze Layer (Raw Ingestion)
Data ingestion is implemented using the Copy Data activity in Fabric pipelines. With Shortcuts, Fabric supports virtualization—allowing data to be accessed from multiple sources without physically copying it into its own storage, improving efficiency. For this demo, a sample dataset from Fabric was ingested into the Bronze layer.
# Silver Layer (Cleansed & Structured Data)
At this stage, the focus is on data quality and usability. The pipeline connects the Bronze layer output to a notebook that performs cleansing tasks such as handling duplicates, resolving null values, formatting columns, and restructuring the data. The processed data is then stored as Delta tables, making it more consistent, reliable, and optimized for analytics.
# Gold Layer (Business-Ready Data)
The Silver layer output is further refined in a second notebook, producing curated datasets tailored for reporting and advanced analytics. This layer delivers trusted, business-ready insights, enabling easy consumption for dashboards, visualization, and decision-making.
# Key Outcome
With Fabric’s integration of pipelines, notebooks, and storage features, this project delivers a streamlined end-to-end data pipeline that demonstrates the Medallion Architecture in action—transforming raw source data into analytics-ready, high-value datasets.
# Note: 
Silver and Gold Layers notebooks attacehd, further screenshots of overall workflow are available in 'MsFabric_Screenshots' folder.
