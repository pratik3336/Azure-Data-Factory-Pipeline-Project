# Azure-Data-Factory-Pipeline-Project

Azure Data Factory Dynamic Pipeline Project using Finance and Education datasets

## Overview

This project is designed focuses on Azure Data Factory (ADF) for data integration and automation. The core task involves creating a dynamic pipeline in ADF to automate the loading of CSV files with various delimiters into a target table in an Azure SQL Database.

### Prerequisites

- Access to Azure SQL Database.
- Access to Azure Data Lake Storage Gen2 (ADLS2).
- Access to Azure Data Factory (ADF).

# Azure Data Factory Configuration

Lookup Activity: Create a Lookup activity in ADF to read the rows from the File_Loading_List table.

ForEach Activity: Utilize the result set from the Lookup activity to drive a ForEach activity, iterating over each file configuration.

Copy Activity: Inside the ForEach loop, configure a Copy activity to read each CSV file based on its specified delimiter and load the data into the corresponding target table.

<img width="407" alt="image" src="https://github.com/pratik3336/Azure-Data-Factory-Pipeline-Project/assets/76115015/3a5fb567-7e11-4676-85bb-6255d60e4291">

<img width="411" alt="image" src="https://github.com/pratik3336/Azure-Data-Factory-Pipeline-Project/assets/76115015/10bd567b-33bd-4036-bb09-5c9a262bf268">
