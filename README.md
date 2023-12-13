# Reorder Analysis Project

## Overview

This project involves the analysis of reorder data in a retail context. The primary objective is to process and analyze sales data, inventory reports, and SKU details to inform restocking decisions. The analysis pipeline is built using R and connects to a SQL Server database to fetch required data. Key operations include data cleaning, transformation, aggregation, and visualization.

## Installation

### Prerequisites

- R and RStudio
- Access to SQL Server with necessary permissions
- Required R packages: `RPostgreSQL`, `dplyr`, `dbplyr`, `data.table`, `lubridate`, `reshape2`, `stringr`, `readxl`, `writexl`, `openxlsx`, `tidyverse`, `odbc`

### Setup

1. **Install R and RStudio**: Download and install R from [CRAN](https://cran.r-project.org/) and RStudio from [RStudio Download](https://rstudio.com/products/rstudio/download/).

2. **Install Required Packages**: Open RStudio and install the required packages by running the following command in the console:

   ```R
   install.packages(c("RPostgreSQL", "dplyr", "dbplyr", "data.table", "lubridate", "reshape2", "stringr", "readxl", "writexl", "openxlsx", "tidyverse", "odbc"))
   ```

3. **Database Connection**: Ensure you have the necessary credentials and network access to connect to the SQL Server.

## Usage

1. **Configure Database Connection**: Modify the database connection details in the script with your SQL Server information (host, database, user ID, and password).

2. **Data Files**: Place any required CSV files in the specified directory and update the file paths in the script accordingly.

3. **Run the Script**: Open the R project and execute the scripts in the RStudio environment. The scripts are organized sequentially from data loading to final data writing.

4. **Output**: The final output will be an Excel file containing the aggregated and analyzed reorder data.

## Additional Notes

- Ensure that the SQL queries used in the script match the schema and tables present in your SQL Server database.
- The script includes data cleaning and transformation steps tailored to the specific structure of the input data. Adjust these as necessary for your dataset.
- The analysis parameters like time frames, SKU details, and inventory levels can be modified to fit different analytical needs.
