# Project Architecture
<img width="989" height="319" alt="image" src="https://github.com/user-attachments/assets/ef17d9ea-2963-4aa2-94c2-9e2497f8eff6" />


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
<img width="466" height="368" alt="image" src="https://github.com/user-attachments/assets/d3a5924f-ef48-4b49-a45f-ee1e0cd7fc4c" />

**STEP 4** => Launch Databricks Workspace      
a. Create compute     
b. Create a folder in the Databricks workspace      
c. Run the given code (Project Documentation) to access data in the data lake     
d. Read the data from all folders/csv file     
e. Perform transformations to the dataset as per requirement    
f. Write the data to MS Azure (**SILVER** container)   

**STEP 5** => Create managed DELTA tables (**GOLD** layer)   
**STEP 6** => Connect to Power BI usning Partner Connect
<img width="940" height="247" alt="image" src="https://github.com/user-attachments/assets/4a35784f-ca17-4bf7-8ae6-889aded75a84" />

