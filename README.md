# Excel: Kickstarter Campaigns Analysis

## Excel Pivot Tables and Pivot Charts

This project required me to organize and analyze a database of 4,200 past Kickstarter campaigns to incover any hidden trends. Kickstarter has been hugely successful as a crowdfunding service, but all of the projects have not seen success. To get funded through a Kickstarter project, the funding must be equal to or greater than the orignal set goal. Only one third of all Kickstarter campaigns find enough funding to go into production. For this reason, companies will spend months researching past projects to uncover successfull trends.  

### Task 1: Organize / Stylize Dataset

For this section of the challenge, I had to modify the provided table with the use of conditional formatting and column creation. The table had to be readable in such a way as to identify market trends. In order to better analyze the data, I added color to cells for clearer identification of differences. To more accurately identify trends, I added percent funded, category, sub-categoy, date created conversion and date ended conversion columns. The steps I took to create the Excel Table are as follows.
* Use conditonal formatting and fill the "state" column cells with colors for successful, failed, canceled or live projects.
* Create column in letter O, name it "Percent Funded" and use a formula to display how much money each campaign made. 
* Use conditional formatting on the Percent Funded column and apply a three-color scale of red, green and blue.
* Create column in letter P, name it "Average Donation" and have it calculate each campaigns average pledge.
* Create columns in letters Q and R, name them "Category" and "Sub-Category".
* Create a formula to seperate the sub-category from category and place them in the corresponding column.
* Create columns in letter S and T, name them "Date Created Converstion" and "Date Ended Conversion".
* Create a formula that converts the Unix Timestamp in launched_at and deadline columns to normal dates and place into the appropriate column.

<p align="center">
    <img width="700" alt="level1" src="https://github.com/mathewqpmiller/Excel-KickstarterAnalysis/blob/main/MDScreenCaptures/RawDataCapture.JPG?raw=true">
</p>

### Task 2: Create Category Pivot Table / Pivot Chart

Now that the original dataset was modified to better identify Kickstarter campaign trends, I now had to create some visualizations to communicate what those trends are. First I had to make a stacked pivot bar chart that looked at the categories of the projects. The steps I took to create the category pivot table and pivot chart are as follows.
* Create a new sheet in the workbook and name it Kickstarter Categories.
* Add a pivot table to the new sheet that analyzes the orignal worksheets category column.
* Count how many of the category projects were successful, failed, canceled or are still active (live).
* Create a, filterable by country, stacked column pivot chart based on the created pivot table. 

<p align="center">
    <img width="700" alt="level1" src="https://github.com/mathewqpmiller/Excel-KickstarterAnalysis/blob/main/MDScreenCaptures/CategoryCapture.JPG?raw=true">
</p>

### Task 3: Create Sub Category Pivot Table / Pivot Chart

Similarly to task two, I had to create a visualization that communicated the success rate of the sub-categories in Kickstarter campaigns. For this I had to make a stacked bar pivot chart, similarly to the category chart, that looked at the sub-categories of categories in the Kickstarter campaigns. The steps I took to create the sub-category pivot table and pivot chart are as follows.
* Create a new sheet in the workbook and name it Kickstarter Sub-Categories.
* Add a pivot table to the new sheet that analyzes the original worksheets sub-category column.
* Count how many of the sub-category projects were successful, failed, canceled or are still active (live).
* Create a stacked column pivot chart of the sub-categories that is filters the pivot table by country and parent-category.

<p align="center">
    <img width="700" alt="level1" src="https://github.com/mathewqpmiller/Excel-KickstarterAnalysis/blob/main/MDScreenCaptures/SubCategoryCapture.JPG?raw=true">
</p>

### Task 4: Create Timeline Pivot Table / Pivot Chart

For this task I had to create a timeline of the Kickstarter campaigns. The purpose of the timeline was to communicate how many campaigns were successful, un-successful or canceled over a period of time. Further, the timeline needed to be filterable by category and year to better understand how these affected the overall trend. The steps I took to create the timeline pivot table and pivot chart are as follows.
* Create a new sheet in the workbook and name it Kickstarter Timeline
* Add a pivot table to the new sheet that analyzes the original worksheets state column and corresponding Date Created row.
* Create a multi-line pivot chart, based on the pivot table, that is filterable by year and category.
th a pivot table with a column of state, rows of Date Created Conversion, values based on the count of state, and filters based on parent category and Years.
Now create a pivot chart line graph that visualizes this new table.

<p align="center">
    <img width="700" alt="level1" src="https://github.com/mathewqpmiller/Excel-KickstarterAnalysis/blob/main/MDScreenCaptures/TimelineCapture.JPG?raw=true">
</p>

### Task 5: Create Success Rate Vs Funding Goal Chart

I now had to create another visualization that would communicate the percent of successful projects vs the orignal set goal for funding. 
In order to do this I had to create a new sheet with 8 columns.  The columns needed to be (Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, Percentage Canceled). I then had to create, in the "Goal" column, 12 rows with the headers (Less than 1000, 1000 to 4999, 5000 to 9999, 10000 to 14999, 15000 to 19999, 20000 to 24999, 25000 to 29999, 30000 to 34999, 35000 to 39999, 40000 to 44999, 45000 to 49999, Greater than or equal to 50000). Using the COUNTIFS() formula, I needed to count how many successful, failed, and canceled projects were created with goals within the ranges listed above. Then I populated the Number Successful, Number Failed, and Number Canceled columns with this data. After that I added up each of the values in the Number Successful, Number Failed, and Number Canceled columns to populate the Total Projects column. Using a mathematical formula, I found the percentage of projects that were successful, failed, or canceled per goal range. With the new set of data, I then created a line chart that graphed the relationship between a goal's amount and its chances at success, failure, or cancellation.

<p align="center">
    <img width="700" alt="level1" src="https://github.com/mathewqpmiller/Excel-KickstarterAnalysis/blob/main/MDScreenCaptures/BonusCapture.JPG?raw=true">
</p>

### Task 6: Final Analysis and Recommendations

Create a report in Microsoft Word and answer the following questions. Given the provided data, what are three conclusions we can draw about Kickstarter campaigns? What are some limitations of this dataset? What are some other possible tables and/or graphs that we could create? Please click on the link http://bit.ly/KickstarterAnalysisReport to see my complete report with a full analysis of my findings.

<p align="center">
UNIVERSITY OF OREGON: Data Analytics Boot Camp - Repository for project 1(Excel Challenge)
</p>
<p align="center">
Mathew Miller © 2021. All Rights Reserved.
</p>
