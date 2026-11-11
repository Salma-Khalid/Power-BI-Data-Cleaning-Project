# Power-BI-Data-Cleaning-Project

## Project Overview
This project focuses on cleaning and preparing a CSV dataset using **Power BI and Power Query**.

The objective is to improve data quality, ensure consistency, remove duplicate records, and prepare a structured dataset for further analysis and visualization.

## Tools & Technologies
- Microsoft Power BI
- Power Query
- Power Query M Language

## Dataset Description
The dataset contains information about top instagram accounts, including:

- `username`: Account username
- `followers`: Number of followers
- `name`: Account name
- `category`: Account category
- `country`: Country associated with the account
- `type`: Account type
- `rank`: Account ranking
- `countries`: Country-related information

*Dataset source: (https://www.kaggle.com/datasets/arkhiplisitsa/instagram-top-accounts).*

## Data Cleaning Process

The following transformations were performed using Power Query:

1. **Data Import**
   - Imported the CSV file .
   - Configured comma as the column delimiter.

2. **Header Transformation**
   - Promoted the first row to column headers.

3. **Data Type Standardization**
   - Converted columns to appropriate data types:
     - Date
     - Text
     - Whole Number (Int64)

4. **Column Removal**
   - Removed unnecessary columns: `also_in` and `date`.

5. **Error Handling**
   - Removed rows containing errors in the `countries` column.

6. **Blank Rows Removal**
   - Eliminated completely empty rows.

7. **Duplicate Removal**
   - Removed duplicate records based on `username`.
   - Applied an additional duplicate removal step based on `rank`.

8. **Data Filtering**
   - Excluded records with missing or empty `country` values.

## Final Dataset
The cleaned dataset retains 8 columns:

`username`, `followers`, `name`, `category`, `country`, `type`, `rank`, `countries`.

The final output is available in CSV format and as a Power BI project file.

## Project Files
| File | Description |
|---|---|
| `cleaned data.pbix` | Power BI project containing the data transformation workflow |
| `cleaned data.csv` | Final cleaned dataset |

## Key Skills Demonstrated
- Data Cleaning & Preparation
- Data Quality Management
- Data Type Transformation
- Duplicate Detection
- Missing Value Handling
- Power Query
- Power Query M Language

---

**Author:** Salma Khalid  
**Tool:** Microsoft Power BI
