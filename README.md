# Blinkit Sales Analysis

#### Dashboard File (24 KB) : https://drive.google.com/drive/folders/1MD9m8JhOYF2Oipp9HkPYkk5o3p4lPo-y?usp=sharing

## Problem Statement

To conduct a comprehensive analysis of Blinkits sales performance, customer satisfaction & inventory distribution to identify key insights & opportunities for optimization using various KPI's & visualizations in Power BI.

### Steps in Project

- Step 1 : Requirement Gathering/ Business Requirements
- Step 2 : Data Walkthrough
- Step 3 : Data Cleaning/Quality Check
- Step 4 : DAX Calculations
- Step 5 : Dashboard/ Report Development


### 1. Requirement Gathering :

KPI's are good at high level of analysis but if we really want to get insights at a deeper level we need to have chart requirements.

-   a. Total Sales by Fat Content : Analyze the impact of FAT content on total Sales.
-   b. Total Sales by Item type : Identify performance of different items on total sales.
-   c. Fat Content by Outlet for Total Sales  
-   d. Total Sales by Outlet establishment : Evaluate how the age or type of outlet establishment influences total sales.  
-   e. Sales by Oulet size : Correlation between oulet size & total sales
-   f. Sales by geography 
-   g All KPI's  broken down by diffrent outlet types.

### 2. Data Walkthrough :

Now the actual first step comes that is to load the data from into Power BI.

Total Rows : 8500

Total Columns : 12 
(Item Fat Content, Item Identifier, Item Type, Outlet Identifier, Outlet Location Type, Outlet Size, Outlet Type, Item Visibility, Item Weight, Sales, Ratings)

Data set Link : https://drive.google.com/drive/folders/1MD9m8JhOYF2Oipp9HkPYkk5o3p4lPo-y?usp=drive_link

### 3. Data Cleaning :

The most important step & my presonal favourite is Data quality check.

Errors/mistakes in the data : Item Fat Content Column having 2 values 'Low Fat' & 'High Fat', but somefields entries were 'LF' or 'HF'. 
For this purpose I used **Power Query Editor** to replace the values, where we can Edit/transfrom the data &then load.

For Data Quality check, in **View** tab, I used **Column Quality** to check the error & empty vlaues in the data.

### 4. DAX Opeartions :

    Average Rating = AVERAGE('BlinkIT Grocery Data'[Rating])
    
    Average Sales = AVERAGE('BlinkIT Grocery Data'[Sales])
    
    No. of Items = COUNTROWS('BlinkIT Grocery Data')
    
    Total Sales = SUM('BlinkIT Grocery Data'[Sales])

  
### 5. Dashboard Designing :

For visualizing the data, metrics created with the help of DAX queries were used. 

I used _New Cards, Stacked Bar Charts, Donut Charts, clustered bar charts, funnel, Matrix & line Charts_ to visualize the data.

![image](https://github.com/user-attachments/assets/0191d19f-b58c-41f3-833d-edf6890eddf0)

