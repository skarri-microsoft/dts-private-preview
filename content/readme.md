# Azure CosmosDB Data Transfer Service Private Preview Tutorials 

This book contains tutorials that demo how to use data transfer service to export and import of data from Azure CosmosDB Cassandra API using Azure Storage using Managed Identity.

## **Prerequisites**

To start tutorials, you would need to have Azure Subscription with 'Data Transfer Capability', if you don't have one, please email shwetn@microsoft.com and skarri@microsoft.com with your subscription id.

Note: There is a charge associated with this service and shows up on your invoice as 'Cluster compute', if you have more billing questions which will be addressed in the email.

If you don't have an Azure subscription, create a <a href="https://azure.microsoft.com/free/?WT.mc_id=A261C142F" data-linktype="external">free account</a> before you begin.</p>

### **Tools**

- <a href="https://docs.microsoft.com/en-us/sql/azure-data-studio/download-azure-data-studio?view=sql-server-ver15" data-linktype="external"> Azure Studio </a> (Note: Samples use Powershell and Python 3 kernals, please ensure these kernal dependencies are installed before running the samples)

### **Azure Resources**

- Azure CosmosDB Cassandra API Account, if you don't have one <a href="https://docs.microsoft.com/en-us/azure/cosmos-db/free-tier" data-linktype="external"> Create a free account </a> 
- Azure Storage Account, if you don't have one <a href="https://docs.microsoft.com/en-us/azure/storage/common/storage-account-create?tabs=azure-portal" data-linktype="external"> click here </a>

- Azure Cosmos DB Cassandra API Table, if you don't have one, please use this notebook to setup [sample data](tutorials/cassandra-sample-data-setup.ipynb)

### **Enable Managed Idendtity between Azure CosmosDB Account and Azure Storage Account**
- Data transfer uses Managed Identity to access Azure storage account. This is required for enteprise security and to avoid keys. please [click here](tutorials/managed-identity.ipynb) and complete this setup.

### **Provision a Data Transfer Service Cluster**
- please [click here](tutorials/provision-data-transfer-service.ipynb) and complete this before tyring export and import. Data transfer service uses this cluster to perform export and import operations.

### **Export/Import data between Azure CosmosDB Cassandra Account and Azure Storage**

- please [click here](tutorials/export-import-sample.ipynb) and follow instructions in the notebook.

### **Usecases**
- Migrate table from shared throughput to dedicated throughput vice versa.
- Change partition key (Note: Schema of the Source and Destination must be same).
- Migrate table with more rus to smaller rus to reduce foot print underneath it.
- Longer retention backups in Avro format for auditing purpose.
