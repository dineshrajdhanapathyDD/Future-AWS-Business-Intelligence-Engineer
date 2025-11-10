

Amazon QuickSight provides a rich set of tools to take organizational data, and make it easier to understand, and use to drive smart business decisions. Now we’re going to let you get introduced to Amazon QuickSight. In this exercise, you’ll perform tasks to begin the process of analyzing a dataset for a business that sells equipment for the roller-skating industry. You'll load data into QuickSight's internal storage, do some initial data preparation, and then build the two foundational resources of a QuickSight project: a Dashboard, and the underlying Analysis on which that Dashboard is based. Once you've practiced these skills, you can begin assessment of any organization's data, from a variety of sources, shaping it to support important business goals. And you'll be ready to accelerate the those processes with the integration of Amazon Q!

Try the following steps:

1.  In the QuickSight left navigation area, select Datasets
2.  Select NEW DATASET
3.  In Create a Dataset, select Upload a file
4.  Select RollerSkateSales.csv
5.  In the Confirm file upload settings window, select Edit Settings and Prepare Data
6.  Rename the ‘name’ field to ‘Customer Name’ using the following steps:
7.  In the Fields area, select the three dots for name, and select Edit name & description
8.  Change Name from ‘name’ to ‘Customer Name’
9.  Select Apply
10.  Repeat these steps to rename ‘currency’ to ‘Purchase Amount’
11.  Repeat these steps to rename ‘color’ to ‘Product Color’
12.  Repeat these steps to rename ‘model’ to ‘Skate Model Name’
13.  Repeat these steps to rename ‘numberOfCustomizations’ to ‘Number of Customizations’
14.  In Fields, select the + button, and select Add calculated field
15.  In Add name, enter ‘High-value Customer’
16.  Provide the following calculation for this field: ifelse({Purchase Amount} > '200', "Yes", "No")
17.  Select SAVE
18.  Select SAVE & PUBLISH
    1.  Select the QuickSight logo in the upper left, and then select Analyses
19.  Select New analysis, and then select the RollerSkateSales dataset
20.  Select USE IN ANALYSIS, and then select CREATE in the New Sheet window
21.  In Visuals, select the Vertical Bar Chart visual
22.  In X AXIS, select Product Color
    1.  In Value, select Purchase Amount
23.  In Group/Color, select Skate Model Name
24.  In the upper right, select PUBLISH
25.  In Dashboard Name, enter ‘Roller Skate Sales Dashboard’, and select PUBLISH DASHBOARD