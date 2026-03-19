# Azure Basics Notes

<p style="text-align: right; font-style: italic">(Completed on Day 2)</p>

## Why Azure exists
Azure exists so companies can use computing resources over the internet instead of buying and managing everything themselves on local servers. It gives access to services like storage, virtual machines, databases, and networking. This makes it easier to scale, deploy faster, and pay only for what is needed.

## Subscriptions
A subscription is the main billing and management boundary in Azure. It is the container that resources are billed under, and it helps organise ownership, costs, and access. A company can use multiple subscriptions to separate environments, teams, or projects.

## Resource groups
A resource group is a logical container for related Azure resources. For example, a data project might place its storage account, data factory, and other related services in one resource group. This makes resources easier to manage, monitor, and delete together if needed.

## Storage accounts
A storage account is the top-level Azure resource that gives access to Azure storage services. It can hold blobs, files, queues, and tables. In a data project, a storage account is often used to store raw files, transformed files, or other data needed by pipelines and analytics tools.

## RBAC
RBAC stands for Role-Based Access Control. It is how Azure controls who can do what on resources. For example, one person might only be allowed to view a storage account, while another can create or delete resources. RBAC helps keep access secure and controlled.

## Azure Data Factory (ADF)
Azure Data Factory is a managed Azure service for moving and orchestrating data. It is used to build pipelines that connect to data sources, copy data, and run transformation steps.

## Azure Databricks
Azure Databricks is a managed analytics service based on Apache Spark. It is commonly used for large-scale data processing, transformation, and engineering work.

## How these fit together in a data project
In an Azure data project, the company would typically have a subscription that contains the project resources. Those resources could be grouped together inside one resource group. A storage account might hold the raw and cleaned data files. Azure Data Factory could move and orchestrate the data. Azure Databricks could transform the data for reporting or analysis. RBAC would control which team members are allowed to view or manage each part.