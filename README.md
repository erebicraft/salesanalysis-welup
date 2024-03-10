# Sales Dashboard 2015- 2017 #
## Project Overview ##
This sales dataset was utilized as part of an Excel assessment to evaluate proficiency in preparing, processing, and analyzing sales data to generate meaningful reports and insights. Throughout this assessment, I delved into Power Pivot and Power Query to enhance data manipulation capabilities.

![Sales Analysis Dashboard](https://github.com/erebicraft/salesanalysis-welup/blob/main/Dashboard%202015%20to%202017.png)

## Data Preparation ##
The dataset used for this project was an [xlsx file](https://docs.google.com/spreadsheets/d/1wLW1QbwluIELVR_ZxCRacCT1IP8Hsoia/edit#gid=350007657) obtained from [Welup Digital Academy](https://welupdigital.com/), comprising 9972 records and 7 fields.

## Tool Used ##
Microsoft Excel served as the primary tool for the entire process.

## Data Process ##
Data cleaning procedures were executed to prepare the dataset for analysis, including:

- Identifying and removing duplicates: 79 duplicates were detected and eliminated.
- Correcting typos and errors: For instance, "Sunbell*" was rectified.
- Handling Outliers: No outliers were discovered
among others

## Data Process ##
In my exploration of Power Pivot and Power Query, I extracted sales data from the dataset based on various years and saved them into a folder named "Sales Folder". Next, I imported the Sales data folder through "Get Data" into the Power Query Editor, where the data was transformed and loaded into Power Pivot tables. 
To explore more, the following step were also carried out:
 
  - Tables for Products, Region, Sales Representatives were created.
  - Data modeling 
 
![Data Modeling](https://github.com/erebicraft/salesanalysis-welup/blob/main/Power%20Pivot%20Modelling%20.png)

## Exploratory Data Analysis ##
This report presents an EDA of the sales data to uncover insights into the company's performance.  These insights aimed to answer key questions, such as
- how is the overall sales trend of the Company?
- what are the top three products?
- who are the most productive sales representatives in 2015, 2016 and 2017 respectively?

## Data Analysis Techniques ##
Various data analysis techniques were employed to extract meaningful insights from the sales data. Notably, pivot tables and charts were utlized to facilitate the analysis process.

![Pivot Tables Used for the Analysis](https://github.com/erebicraft/salesanalysis-welup/blob/main/Pivot%20Table%20Analysis%20Tables%20.png)

- Dax Calculation of total revenue for the year 2015
```excel
TotRev2015:=CALCULATE([Sum of Revenue],Calendar1[Year]=2015)
```
- Derivation of quarter information from the month numbers:
```excel
QtrNo = INT(([Month Number]+2)/3)
```
-Derivation of quarter information from the Quarter Numbers: 
```excel
Qtr = "Qtr"&[QtrNo]
```
## Results / Findings ##
1. ### Overall sales trend ###
 Analysis revealed a consistent upward trend in revenue from the second quarter to the fourth quarter, followed by a sharp decline thereafter.
   
 ![Sales Trend](https://github.com/erebicraft/salesanalysis-welup/blob/main/Sales%20Trend.png)  
   
 2. ### Top three products ###
 The top three revenue-generating products were Quad, Bellen and Doublers with over $193360, $167171 and $148463 respectively as revenue.
 ![Top 3 Products by Revenue](https://github.com/erebicraft/salesanalysis-welup/blob/main/Top%203%20products%20by%20Revenue.png)

 3. ### Most Productive Sales Representaives ###
In 2015, Julie emerged as the most productive sales representative, achieving sales of over $5,827. In 2016, Mike led with sales exceeding $104,108, while in 2017, Julie maintained her top position with sales surpassing $99,145.

![Most Productive SalesRep](https://github.com/erebicraft/salesanalysis-welup/blob/main/Most%20Productive%20Salesrep%20for%20each%20year.png)

## Recommendations ##
Based on the analysis, the following recommendations are made:
- ### Forecasting and Planning ### : The need to ulitize a forecasting models to ascertain future revenue trends and develop strategic plans to mitigate the impact of any potential downward trends and capitalise on upward trends.
- ### Optimization of Cost ###: The need to review and optimaze the company's operational costs is crucial. This involves identifying areas where expenses can be reduced without sacrifiscing quality.
- ### The Most Productive Sales Representatives (Juie and Mike) should awarded for their outstanding performance.

