# dw-project

## Project Description

This project focuses on building a complete Data Warehouse and ETL pipeline using different data integration and business intelligence tools.

### Main Topics
Each team should:

- Extract data from a dataset
- Perform data transformation
- Load data into destinations
- Construct a Star Schema
- Analyze the data using Power BI
- Write project documentation

---

## Detailed Requirements

- Each team should select a dataset from the Internet.
- Each team will be assigned a specific category for the dataset.
- The dataset can be in any format such as Excel, CSV, flat files, etc.

### ETL Process

- Use Alteryx to split the dataset records into two equal halves without using the total number of records directly.
- Load each half into a different destination:
  - First Half → Processed using Alteryx
  - Second Half → Processed using SSIS
- Both destinations for the halves should initially be in Excel format.

### Required Transformations

The same transformations must be applied to both halves using their assigned tools (Alteryx and SSIS):

1. Filter records based on a custom condition.
2. Convert the first character of a string column to uppercase only.
3. Split one column into multiple columns (example: splitting a date column).
4. Replace white spaces with underscores in a string column.

### Data Splitting

Based on the filtering condition:

- The first half will be divided into:
  - Part 1
  - Part 2

- The second half will also be divided into:
  - Part 1
  - Part 2

### SQL Server Destinations

Two SQL Server destinations should be created:

- Destination 1:
  - Load Part 1 from both halves

- Destination 2:
  - Load Part 2 from both halves

---

## Star Schema

- Design a Star Schema with at least:
  - 1 Fact Table
  - 2 Dimension Tables
- Load data from one of the SQL Server destinations into the Star Schema.

---

## Power BI Analysis

Use Power BI to:

- Create at least 3 charts or dashboards
- Apply suitable DAX functions based on the dataset and analysis requirements

---

## Documentation Requirements

The documentation should include:

- A short description of the dataset and its columns
- The components used in:
  - Alteryx
  - SSIS
- Screenshots for each component used
- Analysis and decisions based on the Power BI charts
