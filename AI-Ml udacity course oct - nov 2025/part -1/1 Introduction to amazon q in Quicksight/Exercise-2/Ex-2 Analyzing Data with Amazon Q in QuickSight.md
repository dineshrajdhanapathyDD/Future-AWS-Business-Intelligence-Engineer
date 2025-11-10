Q Topics are a critical component that brings the power of Amazon Q to bear on your data analytics tasks. In this exercise, you'll explain to Amazon Q which ideas are most important in your dataset by creating Named Entities, and then test the ability to ask Amazon Q about those topics to bring greater understanding of what's happening in the roller skating industry. This will help train Amazon Q to understand the way you use your organization's data, and sets you up to build a narrative that inspires decisionmakers to act on the patterns revealed in your data.

1.  In QuickSight, select Topics
2.  Select NEW TOPIC
3.  In Topic name, enter ‘Skate Sales’, and select Continue
4.  In Select a dataset, select RollerSkateSales, and select Create
5.  Wait for the topic to initialize, and then select the new Skate Sales topic to open it
6.  In the Skate Sales topic, in the Data tab, select Data Fields
7.  In the Synonyms column for Product Color, add an alternate name of ‘Skate Color’
8.  In the Synonyms column for Skate Model Name, add alternate names of ‘Model’ and ‘Skate Type’
9.  Select the NAMED ENTITY tab, and then select ADD NAMED ENTITY
10.  Create a named entity called Customer, using the following fields, and then select Save:

-   Address
-   Country
-   Phone
-   PostalZip
-   High-value Customer
-   Customer Name

11.  Select Close, and then select the NAMED ENTITY tab
12.  Create a named entity named Purchase using the following fields, and then select Save:

-   Skate Model Name
-   Product Color
-   Number of Customizations
-   Purchase Amount
-   Customer Name

13.  Select Close
14.  Select the Ask a question about Skate Sales area in the Q Bar
15.  Enter the question: “What color of skate has the most total purchases?”
16.  Mark the interpretation of the question as Verified
17.  Enter the question: “Which country has the most customers?”
18.  Mark the interpretation of the question as Verified
19.  Enter the question: “How many customizations do high-value customers make?”
20.  Change the interpretation of the question to use Average aggregation for Number of Customizations
21.  Mark the interpretation of the question as Verified
22.  Dismiss the Q&A window with the button in the upper right
23.  Select the Suggested Questions tab, and confirm that the Verified questions are present
24.  Select the AI GENERATED tab, and confirm that other question ideas are displayed