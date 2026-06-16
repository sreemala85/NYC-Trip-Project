# Project Architecture

**STEP 1** => Download only TaxiZone Lookup table (csv format). 
**STEP 2** => Creating Azure resources in MS Azure
**Resources created** -
a. Resource Group
b. Storage Account
c. Containers - Bronze & Silver
d. Azure Data Factory workspace
e. Databricks workspace
f. Microsoft Entra Id

**STEP 3** => Launch ADF workspace to ingest raw data from Github to ADLS (**BRONZE** container)
**STEP 4** => Launch Databricks Workspace      
a. Create compute     
b. Create a folder in the Databricks workspace      
c. Run the given code (Project Documentation) to access data in the data lake     
d. Read the data from all folders/csv file     
e. Perform transformations as per requirement    
f. Write the data to MS Azure (**SILVER** container)   

**STEP 5** => Create views from the silver data (**GOLD **layer)
**STEP 6 ** => Connect to Power BI usning Partner Connect
