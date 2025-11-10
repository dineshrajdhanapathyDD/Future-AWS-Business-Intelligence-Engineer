Our first dashboard was a big hit with upper management, and they provided some great ideas to make more business tools like it. Let’s look at the techniques of refining an existing dashboard, and we'll leverage Amazon Q to help make that task easier. We’ll use one of QuickSight’s sample datasets to provide data for this exercise. You'll build an analysis with visuals created with the help of Amazon Q, and then use Q again to help edit those visuals to achieve the exact look and feel that management wants. Once that's done, it's time to publish that analysis as a dashboard.

1.  Open the Topics area in QuickSight
2.  Select NEW SAMPLE TOPIC
3.  Select ‘Clinical Trials’, confirm that Use new generative Q&A experience is selected, and then select CREATE SAMPLE TOPIC
4.  Wait several minutes while the sample topic is created.
5.  Select the QuickSight logo, and select Datasets
6.  Select the Q - Pharmaceutical and Clinical Trials dataset
7.  Select USE IN ANALYSIS, and then select CREATE in the New sheet pane.
8.  In Sheet 1, select the vertical ellipsis button in the AutoGraph visual, and select Delete.
9.  In the Insert menu, select Build visual with Q
10.  In the Build a Visual pane, enter ‘Number of subjects in each state’
11.  Select ‘Add to analysis’
12.  Change the prompt in the Build a Visual pane to: ‘What is the average age of participants in each arm of the study?’
13.  Select ‘Add to analysis’
14.  In the ‘Unique number of Subject Id by State’ visual, select the Edit with Q button.
15.  In the Edit Visual pane, enter: ‘Change visual to vertical bar chart’
16.  In the ‘Unique number of Subject Id by State’ visual, select the Format visual button.
17.  In the Properties pane, in Display Settings, select the brush icon for ‘Edit title’, and edit the title to ‘Subject States of Residence’
18.  Change the ‘Average of Age by Arm’ visual to Vertical Bar Chart
19.  Change the title of the ‘Average of Age by Arm’ title to ‘Average Subject Age by Test Group’
20.  In the ‘Average Subject Age by Test Group’ visual, hover over ‘Arm’ below the chart, and then select the Sort button that appears next to Arm.
21.  In the Properties pane, in X-axis, in Title, edit the title for Arm to ‘Test Group’
22.  Publish the analysis as a new Dashboard named Drug Trial Dashboard, allowing data Q&A.