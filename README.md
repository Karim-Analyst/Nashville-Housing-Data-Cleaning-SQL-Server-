# Nashville Housing Data Cleaning (SQL Server)

## Overview
This project demonstrates the cleaning and structuring of a real-world Nashville housing dataset using SQL Server.
The dataset is prepared to be analysis-ready, with improved consistency and usability.

## Cleaning Steps Performed
### Standardized Dates
Converted `SaleDate` to proper `DATE` format.

### Filled Missing Property Addresses
Used self-joins based on `ParcelID`.

### Split Addresses
Separated property and owner addresses into `Address`, `City`, and `State` columns.

### Standardized Categorical Values
Converted `Y/N` to `Yes/No` in the `SoldAsVacant` field.

### Removed Duplicates
Used `ROW_NUMBER()` with CTEs to identify and remove duplicate records.

### Deleted Unused Columns
Removed unnecessary columns such as `propertyAddress`, `TaxDistrict`, and `OwnerAddress`.

## Folder / File Structure

Nashville-Housing-Data-Cleaning/

│

├── README.md <-- This file

├── sql/

│ └── data_cleaning.sql <-- Cleaned SQL script

├── data/

│ └── nashville_raw_sample.csv <-- Optional small sample of raw dataset


## Dataset
- **Source:** Nashville Housing dataset (real estate)  
- **Domain:** Real Estate / Housing  
- **Tool Used:** SQL Server (T-SQL)  

## Key SQL Techniques Used
- `UPDATE` & `ALTER TABLE`  
- `CONVERT` for date formatting  
- Self-Joins & Joins  
- Common Table Expressions (CTEs)  
- Window Functions (`ROW_NUMBER()`)  
- String Functions (`SUBSTRING`, `CHARINDEX`, `PARSENAME`)  

## Result
The dataset is now clean, structured, and ready for analysis, visualization, or reporting tasks.

## Notes
- A small sample of the raw dataset is included in the `data/` folder for reference.  
- The SQL script in `sql/data_cleaning.sql` contains all steps needed to reproduce the cleaning process.

---
This project highlights practical data cleaning and normalization skills in SQL, suitable for junior data analyst roles.






