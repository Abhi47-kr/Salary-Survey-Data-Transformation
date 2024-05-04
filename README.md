# Data-Cleaning-in-MS-Excel

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tool](#tool)
- [The Cleaning Process](#the-cleaning-process)

## Project Overview

This project aims to transform a disorderly Salary Survey dataset to a clean organised dataset thereby prioritizing data consistency and integrity for seamless analysis and future utilization.

## Data Sources

The primary dataset used for cleaning is a US-centric-ish dataset sourced from AskAManager.org's Salary Survey,  encompassing respondents' demographic and professional information, comprising 19,932 entries across 14 columns.

![Sample](https://github.com/Abhi47-kr/Data-Cleaning-in-MS-Excel/assets/168676103/f864341a-bb5b-4698-a833-587eb20b7434)

## Tool

- Excel

## The Cleaning Process

- Data Backup
  - A copy of the dataset was made in order to have the original dataset in the event of data loss during cleaning.

- Autofit Row Height and Autofit Column Width
  - Implemented autofitting of row height and column width to ensure optimal visibility and readability of data, enhancing user experience and facilitating efficient navigation within the dataset.
 
- Renaming Column Headers
  - Performed renaming of column headers to enhance clarity and usability, ensuring that headers are concise, descriptive, and intuitive for improved data interpretation and analysis.
  - Before
    
     ![Screenshot (14)](https://github.com/Abhi47-kr/Data-Cleaning-in-MS-Excel/assets/168676103/13c837d3-a2e6-4d4a-9c48-2aed9b4fbd68)

  - After
    
     ![Screenshot (16)](https://github.com/Abhi47-kr/Data-Cleaning-in-MS-Excel/assets/168676103/5b732eba-632a-4937-9536-bae8af8a9913)

- Removing Duplicates
  - The dataset was checked for duplicate values and removed accordingly in order to ensure data accuracy.

    ![Screenshot (17)](https://github.com/Abhi47-kr/Data-Cleaning-in-MS-Excel/assets/168676103/6050c447-2c6c-4eb1-846f-e2a2978260d9)

- Data Assessment
  - After assessing the data in order to understand what needed to be done to take it from messy to clean, found out that all 14 columns necessitate varying degrees of refinement to rectify inconsistencies, errors, and formatting issues.

1. **Updating Data Types**
  - Adjusted the data types for all 14 columns: Converted "Salary" and "Additional Salary Compensation" columns from general to numeric data type, ensuring accurate numerical calculations, while switching the remaining columns from general to text data type, facilitating proper handling of textual information and preventing unintended formatting issues.

2. **Standardizing Data Formats**
  - In columns "Overall years of Professional experience" and "Years of experience in field" :
    - Adjusted "1 year or less" to "0-1" to maintain consistency with the format of the other ranges.
    - Removed spaces around the hyphen and "years" to standardize the format, e.g., "21-30" instead of "21 - 30 years" using *Find & Replace*
      
     Before   ![Screenshot (20)](https://github.com/Abhi47-kr/Data-Cleaning-in-MS-Excel/assets/168676103/0c72db82-ce50-48cf-b72e-0c7b1b49bfea)     After   ![Screenshot (22)](https://github.com/Abhi47-kr/Data-Cleaning-in-MS-Excel/assets/168676103/7128703d-3c1f-4b83-af21-518adcbf8b3d)













