# Introduction to end-to-end analytics using Microsoft Fabric
## Introduction
Microsoft Fabric as a comprehensive analytics platform designed to facilitate collaboration between data professionals and business users on data projects. Fabric offers an integrated environment with services for data engineering, data integration, data warehousing, real-time analytics, data science, and business intelligence. It caters to both citizen and professional data practitioners, aiming to provide a unified space for ingesting, storing, processing, and analyzing data. The module introduces the Fabric platform, outlines its target audience, and explores the range of services it encompasses.

## End-to-end analytics with Microsoft Fabric
Microsoft Fabric as a unified and scalable analytics platform that simplifies complex and fragmented analytics processes. Fabric offers persona-optimized experiences through an integrated user interface and operates as a unified software-as-a-service (SaaS) solution, storing all data in a single open format called OneLake.

### OneLake
OneLake is a lake-centric architecture that facilitates collaboration between data professionals and business users on data projects. It eliminates the need to move and copy data between different systems and teams, saving time and streamlining collaboration. OneCopy, a key component of OneLake, enables reading data from a single copy without duplication.

OneLake, built on Azure Data Lake Storage (ADLS), supports various data formats such as Delta, Parquet, CSV, JSON, etc. It acts as a native store for all compute engines in Fabric, including data warehousing, data engineering, data integration, real-time analytics, and Power BI.

### Fabric's Experiences
Fabric's include Synapse Data Engineering, Synapse Data Warehouse, Synapse Data Science, Synapse Real-Time Analytics, Data Factory, and Power BI. These experiences are designed to accomplish specific tasks and seamlessly work together on a single platform, providing a comprehensive data analytics solution.

### Security and Governance
Fabric's security and governance features are highlighted, emphasizing OneLake's central governance and collaboration capabilities. The admin center allows centralized management of groups, permissions, data sources, gateways, and monitoring usage and performance. Fabric is natively integrated with Microsoft Purview Information Protection, using sensitivity labels for classifying and protecting sensitive data throughout the analytics process, from ingestion to export.

## Data teams and Microsoft Fabric
By eliminating data silos and the need for accessing multiple systems, Fabric enhances cooperation between data engineers and data analysts.

Traditionally, the separation between data engineer and data analyst roles required an extra conversation to ensure the data engineer created a suitable data model for the analyst to present data effectively to the business. With Fabric, both roles collaborate within the same Software-as-a-Service (SaaS) product, fostering a better understanding of each other's needs and those of the business. Data analysts gain greater context and the ability to transform data upstream using Data Factory.

Fabric provides a comprehensive experience for data engineers, simplifying data model curation and offering opportunities to expand knowledge with data science techniques. For data analysts, Fabric introduces DirectLake mode, enabling them to directly connect with data lineage and streamline downstream data transformations for Power BI reports.

Data scientists benefit from Fabric's easier integration of native data science techniques, combined with Power BI's interactive reporting, enabling them to provide data-informed insights more effectively.

As a SaaS platform, Fabric allows quick and easy provisioning and execution of various workloads or jobs without pre-approval or planning. This agility enables scaling resources based on changing business needs.

Finally, Fabric introduces the low-to-no-code concept, functionality, and approach to its SaaS offering. While maintaining scale and integrity for data science, data warehousing, data ingestion and prep, and analytics, Fabric provides visual representations of code, making it more accessible and empowering for users.

## Summary 
Data professionals are increasingly expected to be able to work with data at scale, and to be able to do so in a way that is secure, compliant, and cost-effective. At the same time, the business wants to use that data more effectively and quickly to make better decisions. Microsoft Fabric is a collection of tools and services that enables organizations to do just that. In this module, you learned about Fabric's OneLake storage, what workloads that are included in Fabric, and how to enable and use Fabric in your organization.

[<-- Previous](README.md)                                                                                                   [Next -->]()
