# Homework Week 12 - SAS File Export
Bill Kerneckel  
July 28, 2016  



****************************

#### Assignment:

1. Import the following file into SAS. File: dataset1.sas7bdat
2. Export the data to an excel file.
3. Add in State Code to data set
4. Add in the assigned data to the data set (Spending Per Student)
3. Upload the excel file to Github.



****************************
<div id='id-section3.0'/>
#### Instructions

- <strong>Step 1:</strong> Download dataset1.zip file from the Files tab on 2ds.
- <strong>Step 2:</strong> Unzip the file and place "dataset1.sas7bdat" file on your desktop.
- <strong>Step 3:</strong> In SAS goto the Explore tab and locate the "dataset1.sas7bdat" that resides on your desktop.
- <strong>Step 4:</strong> When you open the file "dataset1.sas7bdat" you should see the data appear in your SAS session. The data set should contain 51 rows and 14 columns.
- <strong>Step 5:</strong> Create a new .xls file and save it as "testscores.xls" to your desktop.
- <strong>Step 6:</strong> Plug in the following SAS code and run:

```
proc export 
  data=_EXP0_.DATASET1 
  dbms=xls 
  outfile="\\Client\H$\desktop\testscores.xls" 
  replace;
run;
```
<br>
<strong><u>NOTE</u></strong>
<br>
<br>
Make sure you set the data = in the SAS proc export code to whatever the SAS dataset is called. In this example the dataset was called <strong>"_EXPO_.DATASET1_"</strong>.

****************************

#### Census Data

Since I was assigned "Sudent Per Student" I searched the United States Census Bureau webisite. I came across the following excel tabel:

[https://www.census.gov/govs/school/](https://www.census.gov/govs/school/)


Note: this data is from 2014.

****************************

####  Upload Excel file to github                          

Now that you have the "testscores.xls" file on your desktop you can now upload it to your gitHub.


****************************

#### Modifications to the excel file

I added in two columns to the excel file. The first column "B" is the state abbrivations. The second column "C" is the 2014 data I pulled from the Census website. I did change the format of column "C" to number format since this information is financial data.


****************************

#### Excel File                                                 

To download and view the excel file click on the icon. [![click Here](images/excel.png)](https://github.com/wkerneck/SASFileExport/blob/master/data/testscores.xls?raw=true)



