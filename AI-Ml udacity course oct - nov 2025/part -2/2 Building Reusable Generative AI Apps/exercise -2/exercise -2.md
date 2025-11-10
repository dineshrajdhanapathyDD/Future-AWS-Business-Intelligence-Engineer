Now it’s your turn again. This time you’re going to take your Q Business app, and configure it to support requests from different departments of the company, returning appropriate responses for users in each department.

## Prerequisites

-   You have completed the Setting up the Environment Video in Exercise 1.

## Downloading Exercise Files

-   Course-related files, such as meeting transcripts, will be available for download from the "Download" section.

## Exercise Scenario

-   You have received a request to make your call center employee app customizable to support employees in different company departments.
-   In this exercise, you’ll use Amazon Q Business to create a Customer Complaint Response Generator App and then expand the functionality.

## High Level Steps

1.  Create and Test a Customer Complaint Response Generator App
2.  Add a Card to your Q Business App
3.  Edit the Output Card to Incorporate the Department Input
4.  Test the Application to Verify New Functionality

## Detailed Instructions

### Section 1: Opening Amazon Q Business and Navigating to Your Q Business App

1.  Login to AWS console with required privileges.
2.  Navigate to Amazon Q Business service in correct AWS region.
3.  Select Applications in the navigation area.
4.  In the Applications page, select the link for the Application that was precreated.
5.  On the Application details page of your Application, click on Deployed URL link.
6.  Login using your IAM or IAM Identity Center user credentials.
7.  Select the Apps button in the left navigation

### Section 2: Create a Customer Complaint Response Generator App

1.  Generate an App from the following prompt: "In response to a customer complaint about a product, generate a polite, professional response to be read over the telephone, explaining that the company is committed to making the customer satisfied."
2.  Edit the Response card to confirm that the Input Cards Product Detail and Complaint Detail are used to generate the response.
3.  Confirm that the response is generated from General Knowledge.
4.  Generate a Sample Complaint from the following details:
    1.  Product Details: Super Yello Model 300 Tennis Balls (3-pack)
    2.  Complaint Details: Tennis balls arrived underinflated.
5.  Confirm the response is appropriate to the customer issue.

### Section 3: Adding a Card to your Q Business App

2.  In your Q Business App, select the Add card button, and select a Text Input card type.
3.  Give the card a Title of  _Department._
4.  Give the card a Placeholder of  _Enter the department you work in._
5.  Give the card a default value of  _Customer Service_.
6.  Select the Save button.

### Section 4: Editing the Output Card to Incorporate the Department Input

1.  Edit the Response - Output card.
2.  Edit the Prompt to specify the need to respond as a member of a department to create the polite, professional response. Use an @ in front of the name of your Department input card to include it correctly in the prompt.
3.  Select the Save button.

### Section 5: Testing the Application to Verify New Functionality

1.  Respond to a sample complaint as a member of the Customer Service department, by entering the description of a product and of a complaint in the input boxes, and entering  _Customer Services_  in the department input card, and selecting the Run button.
2.  Confirm that the response is customized to be appropriate for a Customer Service employee.
3.  Change the Department input card to Marketing, and rerun the App.
4.  Change the Department input card to Sales, and rerun the App.
5.  Confirm that the app produces appropriate responses for each input.