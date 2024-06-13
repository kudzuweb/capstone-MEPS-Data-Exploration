# NSS DS7 Capstone Project
*This project downloads data and webscrapes HTML codebooks from the Medical Expenditure Panel Survey(MEPS) from the Agency for Healthcare Research and Quality, then packages selected data into relevant views to feed into Tableau.*

## **Notebooks**

*webscrapecapstonedata* - accesses the webpages for the data for 2012-2021 and downloads the SAS and SASv9 files.

*webscrapecapstonecodebooks* - accesses the pages of variables and the pages for each variable, creates dictionary of dictionaries of lists for each year for each dataset, exports as pickles

*cleanupcapstonedata* - renames files, adds YEAR column, exports CSVs

*cleanupcapstonecodebooks*- merges and concatenates pickles into one frame per year for each dataset, renames, exports CSVs

*RTF Files* - contain SQL queries used in BigQuery to generate the views used to create Tableau dashboard.

***

*insert diagram here*

***

#### **Dataset Links**

[MEPS Full-Year Population Characteristics](https://meps.ahrq.gov/mepsweb/data_stats/download_data_files_results.jsp?cboDataYear=All&cboDataTypeY=1%2CHousehold+Full+Year+File&buttonYearandDataType=Search&cboPufNumber=All&SearchTitle=Population+Characteristics)

[MEPS Hospital Inpatient Stays](https://meps.ahrq.gov/mepsweb/data_stats/download_data_files_results.jsp?cboDataYear=All&cboDataTypeY=2%2CHousehold+Event+File&buttonYearandDataType=Search&cboPufNumber=All&SearchTitle=Hospital+Inpatient+Stays)

[MEPS Emergency Room Visits](https://meps.ahrq.gov/mepsweb/data_stats/download_data_files_results.jsp?cboDataYear=All&cboDataTypeY=2%2CHousehold+Event+File&buttonYearandDataType=Search&cboPufNumber=All&SearchTitle=Hospital+Inpatient+Stays)

[MEPS Office-Based Medical Provider Visits](https://meps.ahrq.gov/mepsweb/data_stats/download_data_files_results.jsp?cboDataYear=All&cboDataTypeY=2%2CHousehold+Event+File&buttonYearandDataType=Search&cboPufNumber=All&SearchTitle=Office-Based+Medical+Provider+Visits)
