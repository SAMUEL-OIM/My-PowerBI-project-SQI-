# Consumer Financial Complaints Analytics

## Overview
This project is focused on improving customer satisfaction, and it describes how consumers rate certain products.


## Aims & Objectives
- When do complaints rise or fall over time?
-	Which states and regions are hotspots?
-	Which products and sub-products drive the most complaints?
-	Which issues and sub-issues are most common or most severe?
-	How fast, and how timely are company responses to complaints?
-	Which companies show the highest complaint rates relative to market share?
-	Do company traits (size tier, reputation, enforcement history) correlate with outcomes?
-	Do submission channels differ in response speed or outcomes?

## Steps Taken:
- Data Gathering
- Data Cleaning
- Data Modeling
- Analyze
- Visualization

## Data Gathering
The data was collected from Onyx Data Source: [Here](https://datadna.onyxdata.co.uk/challenges/october-2025-datadna-consumer-financial-complaints-analytics-challenge/)

The tools used in this project is Microsoft Power BI [Download Here](https://www.microsoft.com/en-us/download/details.aspx?id=58494)

## Data Cleaning
- Trimmed Records: Removed unnecessary leading and trailing spaces across all text fields.
- Extracted Key Information: Extracted years from date fields for easier grouping and analysis.
- Extracted states and countries from address fields to create structured location variables.
- Concatenated for Full Name: Merged first and last name fields into a unified “Full Name” column.
- Fill Down: Filled missing values within grouped datasets to maintain completeness.
- Applied Proper Case: Converted text entries into Proper Case for neat and professional formatting.
- Standardized Data: Cleaned and normalized formats (names, addresses, and codes) to prevent duplicates and ensure consistent representation across the dataset.

## Data Modeling
- Separated the main data table from the lookup tables.
- Created primary key–foreign key relationships across all tables.
- Linked tables using Customer_ID, Product_ID, ProductCategory_ID, ProductSubCategory_ID, Manufacturer_ID, and SalesTerritory_ID
- Ensured correct cardinality (one-to-many or many-to-one) across all relationships.

## Analye
These are the following DAX (Measures) :
- To get the Total no. of complaints
  DAX EXPRESSION
   ```
   Total Complaints = Count('ComplaintsTable', Complaint_ID)
  ```
   - To get the Total no. of Companies
  DAX EXPRESSION
   ```
   Total Companies = Count('ComplaintsTable', Company_ID)
  ```
   
## Visualisation 
<img width="1566" height="884" alt="Screenshot 2025-11-04 095002" src="https://github.com/user-attachments/assets/56be140f-f743-4bf9-9d80-db283033ba66" />
<img width="1534" height="860" alt="Dashboard Page 2" src="https://github.com/user-attachments/assets/3f8e43e3-6df8-484f-9229-c7505c0c5585" />
<img width="1536" height="872" alt="Dashboard Page 3" src="https://github.com/user-attachments/assets/cdbf752f-4546-4e1a-81b7-941ef1ccd054" />

