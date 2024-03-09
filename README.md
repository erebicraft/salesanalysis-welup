# Sales Dashboard 2015- 2017 #
## Project Overview ##
This sales dataset was utilized as part of an Excel assessment to evaluate proficiency in preparing, processing, and analyzing sales data to generate meaningful reports and insights. Throughout this assessment, I delved into Power Pivot and Power Query to enhance data manipulation capabilities.

![Sales Analysis Dashboard](https://github.com/erebicraft/salesanalysis-welup/blob/main/Dashboard%202015%20to%202017.png)

## Data Preparation ##
The dataset used for this project is an [xlsx file](https://docs.google.com/spreadsheets/d/1wLW1QbwluIELVR_ZxCRacCT1IP8Hsoia/edit#gid=350007657) obtained from [Welup Digital Academy](https://welupdigital.com/), comprising 9972 records and 7 fields.

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
The EDA involved exploring the sales data to answer key questions, such as
- how is the overall sales trend of the Company?
- what are the top three products?
- who are the most productive sales representatives in 2015, 2016 and 2017 respectively?

## Data Analysis ##
Here are some of the analysis used 
![Pivot Tables Used for the Analysis](https://github.com/erebicraft/salesanalysis-welup/blob/main/Pivot%20Table%20Analysis%20Tables%20.png)

```excel
TotRev2015:=CALCULATE([Sum of Revenue],Calendar1[Year]=2015)
```
```excel
QtrNo = INT(([Month Number]+2)/3)
```
```excel
Qtr = "Qtr"&[QtrNo]
```




