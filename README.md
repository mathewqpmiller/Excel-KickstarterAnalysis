# Excel: Kickstarter Projects Analysis

## Excel Pivot Tables and Pivot Charts

This project required me to organize and analyze a database of 4,200 past Kickstarter campaigns to incover any hidden trends. Kickstarter has been hugely successful as a crowdfunding service, but all of the projects have not seen success. To get funded through a Kickstarter project, the funding must be equal to or greater than the orignal goal. Only one third of all Kickstarter campaigns find enough funding for a positive outcome. For this reason, companies will spend months researching past projects to uncover successfull trends.  

### Task 1: Organize / Stylize Dataset

For this section of the challenge, I had to modify and analyze the provided table with the use of conditional formatting and column creation. The table had to be readable in such a way as to identify market trends. The steps to create the Excel Table are as follows.
* Use conditonal formatting and fill the "state" column cells with colors for successful, failed, canceled or live projects.
* Create column letter "O", name it Percent Funded and use a formula to display how much money each campaign made. 
* Use conditional formatting on the "Percent Funded" column and apply a three-color scale of red, green and blue.
* Create column letter "P", name it Average Donation and have it calculate each campaigns average contribution.
* Create column letters "Q" / "R", name them Category / Sub-Category and use a formula to split sub-category from category
while placing them into the corresponding cells.

### Task 2: Create Category Pivot Table / Pivot Chart

Now that the original dataset has be altered to better identify trends in Kickstarter campaigns, I now have to create some visualizations to communicate what those trends are.  First I have to make a bar chart that looks at the categorys of the projects.  The steps to create the category pivot table and pivot chart are as follows.
* Create a new sheet in the workbook.
* Add a pivot table to the new sheet that analyzes the orignal worksheet.
* Count how many of the projects are successful, failed, canceled or still active (live) per category.
* Create a, filterable by country, stacked column pivot chart based on the created pivot table 


### Task 3: Create Sub Category Pivot Table / Pivot Chart

Create a new sheet with a pivot table that will analyze your initial sheet to count how many campaigns were successful, failed, or canceled, or are currently live per sub-category.
Create a stacked column pivot chart that can be filtered by country and parent-category based on the table you have created.
The dates stored within the deadline and launched_at columns use Unix timestamps. Fortunately for us, there is a formula that can be used to convert these timestamps to a normal date.
Create a new column named Date Created Conversion that will use this formula to convert the data contained within launched_at into Excel's date format.
Create a new column named Date Ended Conversion that will use this formula to convert the data contained within deadline into Excel's date format.

### Timeline

Create a new sheet with a pivot table with a column of state, rows of Date Created Conversion, values based on the count of state, and filters based on parent category and Years.
Now create a pivot chart line graph that visualizes this new table.
Create a report in Microsoft Word and answer the following questions.
Given the provided data, what are three conclusions we can draw about Kickstarter campaigns?
What are some limitations of this dataset?
What are some other possible tables and/or graphs that we could create?

### Bonus

Create a new sheet with 8 columns:
Goal
Number Successful
Number Failed
Number Canceled
Total Projects
Percentage Successful
Percentage Failed
Percentage Canceled
In the Goal column, create 12 rows with the following headers:
Less than 1000
1000 to 4999
5000 to 9999
10000 to 14999
15000 to 19999
20000 to 24999
25000 to 29999
30000 to 34999
35000 to 39999
40000 to 44999
45000 to 49999
Greater than or equal to 50000
Using the COUNTIFS() formula, count how many successful, failed, and canceled projects were created with goals within the ranges listed above. Populate the Number Successful, Number Failed, and Number Canceled columns with this data.
Add up each of the values in the Number Successful, Number Failed, and Number Canceled columns to populate the Total Projects column. Then, using a mathematical formula, find the percentage of projects that were successful, failed, or canceled per goal range.
Create a line chart that graphs the relationship between a goal's amount and its chances at success, failure, or cancellation.


UNIVERSITY OF OREGON: Data Analytics Boot Camp - Repository for activity 1(Excel Challenge)
