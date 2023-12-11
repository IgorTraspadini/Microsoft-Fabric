# Introduction
Fabric's Lakehouse is built upon the OneLake scalable storage layer and leverages Apache Spark and SQL compute engines for big data processing. A Lakehouse is defined as a unified platform that combines the flexible and scalable storage of a data lake with the ability to query and analyze data similar to a data warehouse.

The scenario presented involves a company that has traditionally used a data warehouse to store structured data from transactional systems. However, challenges arise when dealing with unstructured data from sources like social media, website logs, and third-party platforms, which are challenging to manage and analyze within the existing data warehouse infrastructure. To address this, the company opts for Microsoft Fabric to enhance decision-making capabilities by analyzing data in various formats from multiple sources.

The module explores how the Lakehouse in Microsoft Fabric serves as a solution to such scenarios. It provides a scalable and flexible data store for both files and tables, allowing users to query the data using SQL. This approach enables efficient analysis of diverse data types and sources within a unified platform, offering improved capabilities for decision-making.

## Learning objectives
- Describe core features and capabilities of lakehouses in Microsoft Fabric
- Create a lakehouse
- Ingest data into files and tables in a lakehouse
- Query lakehouse tables with SQL

## Microsoft Fabric Lakehouse
A Lakehouse presents as a database and is built on top of a data lake using Delta format tables. Lakehouses combine the SQL-based analytical capabilities of a relational data warehouse and the flexibility and scalability of a data lake. Lakehouses store all data formats and can be used with various analytics tools and programming languages. As cloud-based solutions, lakehouses can scale automatically and provide high availability and disaster recovery.

Some benefits of a lakehouse include:
- Lakehouses use Spark and SQL engines to process large-scale data and support machine learning or predictive modeling analytics.
- Lakehouse data is organized in a schema-on-read format, which means you define the schema as needed rather than having a predefined schema.
- Lakehouses support ACID (Atomicity, Consistency, Isolation, Durability) transactions through Delta Lake formatted tables for data consistency and integrity.
- Lakehouses are a single location for data engineers, data scientists, and data analysts to access and use data.

After creating a lakehouse, you can load data - in any common format - from various sources; including local files, databases, or APIs. Data ingestion can also be automated using Data Factory Pipelines or Dataflows (Gen2) in Microsoft Fabric.

After you've ingested the data into the Lakehouse, you can use Notebooks or Dataflows (Gen2) to explore and transform it.
Data Factory Pipelines can be used to orchestrate Spark, Dataflow, and other activities; enabling you to implement complex data transformation processes.

After transforming your data, you can query it using SQL, use it to train machine learning models, perform real-time analytics, or develop reports in Power BI.

You can also apply data governance policies to your Lakehouse, such as data classification and access control.

## Work with Microsoft Fabric Lakehouses
### Create and explore a lakehouse
You create and configure a new Lakehouse in the Data Engineering workload. Each lakehouse produces three named items in the Fabric-enabled workspace:

- Lakehouse is the lakehouse storage and metadata, where you interact with files, folders, and table data.
- Dataset (default) is an automatically created data model based on the tables in the lakehouse. Power BI reports can be built from the dataset.
- SQL Endpoint is a read-only SQL endpoint through which you can connect and query data with Transact-SQL.

You can work with the data in the lakehouse in two modes:
- Lakehouse enables you to add and interact with tables, files, and folders in the Lakehouse.
- SQL Endpoint enables you to use SQL to query the tables in the lakehouse and manage its relational data model.

### Ingest data into a lakehouse
There are many ways to load data into a Fabric lakehouse, including:
- Upload: Upload local files or folders to the lakehouse. You can then explore and process the file data, and load the results into tables.
- Dataflows (Gen2): Import and transform data from a range of sources using Power Query Online, and load it directly into a table in the lakehouse.
- Notebooks: Use notebooks in Fabric to ingest and transform data, and load it into tables or files in the lakehouse.
- Data Factory pipelines: Copy data and orchestrate data processing activities, loading the results into tables or files in the lakehouse.

Another way to access and use data in Fabric is to use shortcuts. Shortcuts enable you to integrate data into your lakehouse while keeping it stored in external storage.

Shortcuts are useful when you need to source data that's in a different storage account or even a different cloud provider. Within your Lakehouse you can create shortcuts that point to different storage accounts and other Fabric items like data warehouses, KQL databases, and other Lakehouses.

Source data permissions and credentials are all managed by OneLake. When accessing data through a shortcut to another OneLake location, the identity of the calling user will be utilized to authorize access to the data in the target path of the shortcut. The user must have permissions in the target location to read the data.

Shortcuts can be created in both Lakehouses and KQL databases, and appear as a folder in the lake. This allows Spark, SQL, Real-Time Analytics and Analysis Services to all utilize shortcuts when querying data.

## Explore and transform data in a lakehouse
After loading data into the lakehouse, you can use various tools and techniques to explore and transform it, including:
- Apache Spark: Each Fabric lakehouse can use Spark pools through Notebooks or Spark Job Definitions to process data in files and tables 
  in the lakehouse using Scala, PySpark, or Spark SQL.
  
       - Notebooks: Interactive coding interfaces in which you can use code to read, transform, and write data directly to the lakehouse 
         as tables and/or files.
       - Spark Job Definitions: On-demand or scheduled scripts that use the Spark engine to process data in the lakehouse.
- SQL Endpoint: Each lakehouse includes a SQL endpoint through which you can run Transact-SQL statements to query, filter, aggregate, and otherwise explore data in lakehouse tables.
- Dataflows (Gen2): In addition to using a dataflow to ingest data into the lakehouse, you can create a dataflow to perform subsequent transformations through Power Query, and optionally land transformed data back to the Lakehouse.
- Data Pipelines: Orchestrate complex data transformation logic that operates on data in the lakehouse through a sequence of activities (such as dataflows, Spark jobs, and other control flow logic).

### Analyze and visualize data in a lakehouse
The data in your lakehouse tables is included in a dataset that defines a relational model for your data. You can edit this dataset (or create other datasets), defining custom measures, hierarchies, aggregations, and other elements of a data model. You can then use the dataset as the source for a Power BI report that enables you to visualize and analyze the data.

By combining the data visualization capabilities of Power BI with the centralized storage and tabular schema of a data lakehouse, you can implement an end-to-end analytics solution on a single platform.

## Lab
[Create a Lakehouse](https://microsoftlearning.github.io/mslearn-fabric/Instructions/Labs/01-lakehouse.html)
- Create a workspace
- Create a lakehouse
- Upload a file
- Explore shortcuts
- Load file data into a table
- Use SQL to query tables
- Create a visual query
- Create a report

## Summary
Microsoft Fabric lakehouses provide data engineers and analysts with the combined benefits of data lake storage and a relational data warehouse. You can use a lakehouse as the basis of an end-to-end data analytics solution that includes data ingestion, transformation, modeling, and visualization.

## Source
[Microsoft](https://www.microsoft.com/en-us/microsoft-fabric)

[<-- Previous](Introduction.md)                                                                                             [Next -->]()
