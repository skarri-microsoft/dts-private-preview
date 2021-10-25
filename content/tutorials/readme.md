# Azure CosmosDB Data Transfer Service Private Preview Tutorials 

### **Enable Managed Idendtity between Azure CosmosDB Account and Azure Storage Account**
- Data transfer uses Managed Identity to access Azure storage account. This is required for enteprise security and to avoid keys. please [click here](tutorials/managed-identity.ipynb) and complete this setup.

### **Provision a Data Transfer Service Cluster**
- please [click here](tutorials/provision-data-transfer-service.ipynb) and complete this before tyring export and import. Data transfer service uses this cluster to perform export and import operations.

### **Export/Import data between Azure CosmosDB Cassandra Account and Azure Storage**

- please [click here](tutorials/export-import-sample.ipynb) and follow instructions in the notebook.