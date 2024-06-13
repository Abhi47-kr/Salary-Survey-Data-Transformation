# SALARY SURVEY DATA TRANSFORMATION

![alexander-mils-lCPhGxs7pww-unsplash](https://github.com/Abhi47-kr/Salary-Survey-Data-Transformation/assets/168676103/306fa38c-82a2-4848-a56e-49b609eb5f28)


## TABLE OF CONTENTS

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tool Used](#tool-used)
- [The Cleaning Process](#the-cleaning-process)
- [PROJECT IMPACT](#project-impact)
- [Conclusion](#conclusion)

## PROJECT OVERVIEW

This project aims to transform a disorderly Salary Survey dataset to a clean organised dataset thereby prioritizing data consistency and integrity for seamless analysis and future utilization.

## DATA SOURCES

The primary dataset used for cleaning is a US-centric-ish dataset sourced from AskAManager.org's Salary Survey,  encompassing respondents' demographic and professional information, comprising 19,932 entries across 14 columns. The raw uncleaned data can be viewed [here](https://github.com/Abhi47-kr/Salary-Survey-Data-Transformation/blob/b73c972a1d5055b6be15b527165b76ea9545092a/Dataset.xlsx).

![Sample](https://github.com/Abhi47-kr/Data-Cleaning-in-MS-Excel/assets/168676103/f864341a-bb5b-4698-a833-587eb20b7434)

## TOOL

- Excel (free web version)

## THE CLEANING PROCESS

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
    

3. Formatting "Industry" & "Job Title" columns
  - Standardized Capitalization
    - ensuring all job titles are in a consistent format in title case using *PROPER* function.
  - Removed Leading and Trailing Spaces
    - using *TRIM* function.
      
 - Before ![Screenshot (25)](https://github.com/Abhi47-kr/Data-Cleaning-in-MS-Excel/assets/168676103/136f010c-9276-4e5b-9cd6-bd450330d1b3)
 - After ![Screenshot (24)](https://github.com/Abhi47-kr/Data-Cleaning-in-MS-Excel/assets/168676103/93840ca8-3d10-4a1e-a070-e79184b6c271)


4. **Standardizing "Job Title", "Country", "Currency", "City" & "Race" columns**
  - Grouped similar data points using *FILTER, FIND & REPLACE, IF function, Split Text to Columns* to reduce redundancy.
    - for example "Senior Software Engg", "Sr Software Engineer", and "Sr. Software Engineer" etc under a single category "Senior Software Engineer".
    - also in "Races" Column, for example grouping "Asian or Asian American, Black or African American, Hispanic, Latino, or Spanish origin" to "Asia or Asian American" using first preference priority. And like "Another option not listed here or prefer not to answer" to "Others".
    - grouped same countries with different abbrevations like "U.S", "US.", "U.S.", "U.S.A", to "US"

  - Rectified and deleted inconsistencies among data points in respective columns ensuring uniformity and clarity for streamlined analysis.

    
5. **Filling Empty Cells**
  - Empty cells in columns "Additional Monetary Compensation", "State", "Highest level of Education", "Gender", "Race", were identified using *FILTER*
  - The empty cells was then filled with "NA" using *IF* and *ISBLANK* function.


6. **Removing Inconsistent Data Column**

   ![Screenshot (29)](https://github.com/Abhi47-kr/Data-Cleaning-in-MS-Excel/assets/168676103/715455d6-6fc3-4925-a47f-52cfb44fe0f9)
   
  - Recognizing wide-ranging inconsistencies in the "Additional monetary compensation" column, deemed its contribution to analysis as limited, and proceeded with its deletion to streamline the dataset and focus on relevant variables for meaningful analysis.


7. **Detecting and Removing Outliers**
  - Manually inspected the data to identify potential outliers using *SORTING* and than removed it accordingly from the dataset.
   - Outliers were identified based on extreme values and anomalies, considering the dataset's diverse currency denominations from various countries.
   - Employed a manual approach instead of automated methods like Z-scores or standard deviation due to the currency variations.

### The complete transformed data can be viewed [here](https://github.com/Abhi47-kr/Salary-Survey-Data-Transformation/blob/b73c972a1d5055b6be15b527165b76ea9545092a/Dataset_cleaned.xlsx)

## PROJECT IMPACT
- *Processed 19,932 survey entries* across *14 columns* to ensure data consistency and accuracy.
- *Removed* duplicates to maintain data accuracy, eliminating over *500 redundant entries*.
- *Rectified* and *grouped* over *1,000 similar data points* to reduce redundancy and improve data clarity.
- Detected and manually *removed outliers* based on extreme values and anomalies, ensuring a clean dataset suitable for reliable analysis.

## CONCLUSION

Through a systematic data cleaning process and taking all the necessary steps for cleaning, the data is now ensured for reliable analysis. In addition to this, the feeling of fulfillment is also achieved that comes with transforming a messy dataset to a clean one :smile:

     
  ![Screenshot (31)](https://github.com/Abhi47-kr/Data-Cleaning-in-MS-Excel/assets/168676103/c263d8d5-7344-4363-91ca-632d5ec4b899)

    
    

      







    
    













