## Exercise Scenario

-   You’ve recently joined a new tech company and are attending several onboarding meetings. To keep track, you use the meeting platform’s transcription tool to save the sessions. However, searching these static transcripts manually is time-consuming.
-   In this exercise, you’ll use Amazon Q Business to automatically generate meeting summaries and enable question-answering over the transcripts for easier access to information.

## High Level Steps

1.  Set up AWS IAM Identity Center
2.  Initialize Amazon Q Business
3.  Upload your document and start asking questions in Natural Language

  

## Detailed Instructions

## Section 1: Setting up the Environment

Watch the video below and set up the environment to start working with Q Business.

refer : [Getting Started With Q Business Apps Setup V1](https://www.youtube.com/watch?v=tIwYfgKbnH0)

## Guide to Setting Up Amazon Q with AWS Identity Center

Setting up Amazon Q Business and managing access involves several key steps. Here’s a concise guide:

### Key Steps:

1.  **Configure AWS Identity Center**
    -   Navigate to AWS IAM Identity Center.
    -   Disable multi-factor authentication (MFA) for the lab environment.
    -   Recommend enabling MFA for production environments.
2.  **Grant Application Access**
    -   Return to Amazon Q Business.
    -   Allow access for the career coaches group.
    -   No users or groups are initially associated; add them through the "Groups" option.
    -   Assign existing users to the group.
    -   Verify the group count is updated.
3.  **Reset User Password**
    -   Go back to Identity Center to reset one user’s password.
    -   Generate a one-time password.
    -   Note down this password for login.
4.  **User Login and Finalization**
    -   Use the password to sign into the application.
    -   Set a new memorable password.
    -   Access the application page for Amazon Q Business.

Efficiently manage access and security for smooth operation of Amazon Q Business.

## Section 2: Upload your document and start asking question in Natural Language

1.  On the Application details page of your application, click on Deployed URL link.
2.  Login using your user credentials
3.  Navigate to Amazon Q Business Chat Interface
4.  Upload your document (Sales Strategy Meeting found in Downloads tab)
5.  Start asking questions in natural language after uploading below documents one by one:
    -   Upload Sales Strategy Meeting Transcript and ask below questions:
        1.  Who is leading Central US sales team? ``` Based on the current uploaded file, Tom is the Regional Sales Manager who manages the Central US sales team. This is stated in his introduction during the meeting: "Hey all, Tom here. I manage the Central US sales team."```
        2.  How much is the qualified pipeline for Q2? ```According to the sales strategy meeting transcript, Ellie (Sales Ops) reported that as of the meeting date (April 5, 2025), there was $12.3M in qualified pipeline for Q2, with $4.5M in Commit. ```
        3.  What are top three risks? 
```Based on the sales strategy meeting transcript, the top three risks identified are: 
6. $3.1M of the Commit pipeline has no activity logged in the past 10 business days, which was described as "concerning" by Ellie from Sales Ops.

7. Legal delays with deals like FinTrust, where the legal team has "gone dark" despite the deal being at 80% stage and having cleared InfoSec.

8. Competing vendors ramping up discounts, specifically XCorp offering 20% off if contracts are signed before May 1, creating pricing pressure on deals.
```
      
  4.  How is competition affecting the sales? 
 ```
Based on the sales strategy meeting transcript, competition is affecting sales through aggressive discounting. Specifically, Nina (Enterprise Account Executive) mentioned that "competing vendors are ramping up discounts" and noted that "XCorp is offering 20% off if contracts are signed before May 1," which is "creating some pressure" on their deals.

In response to this competitive pressure, Omar from Finance offered to "authorize pre-approved discounts up to 15% for strategic deals" to help counter the competition's pricing strategy 
```

----
  
   -   Upload Candidate Onboarding Automation Project Meeting Transcript (Candidate Onboarding Automation Project found in Downloads tab) and ask below questions:
        1.  When is project starting? 
  ```
 Based on the current uploaded file (Candidate Onboarding Automation Project – Kickoff Meeting Transcript), the development for the project is scheduled to start on April 11, 2025. This is mentioned in the milestones section where James (Project Manager) proposes:

"· April 8 – Finalize requirements
· April 10 – Approve architecture
· April 11 – Start development
· April 15 – QA setup and test data ready
· April 25 – UAT with HR
· May 5 – Go-live" 
```
        2.  Who is the tech lead?  
 ``` 
Based on the Candidate Onboarding Automation Project kickoff meeting transcript, Ayesha is the Technical Lead. She introduced herself in the meeting saying: "Hey everyone, I'm Ayesha. I'll lead the development side, including architecture, infrastructure setup in AWS, and backend logic. We're aiming for a secure, scalable build." 
```
        
        3.  Which technology is being used?
```
Based on the Candidate Onboarding Automation Project kickoff meeting transcript, the following technologies are being used:

- Backend: Java with Spring Boot
- Database: MySQL on Amazon RDS
- Infrastructure: EC2 instances, S3 for storage
- Email service: Amazon SES
- IAM for access control
- Encryption at rest for data protection

These technologies were outlined by Ayesha, the Technical Lead, when discussing the technical implementation of the project. 
```
        4.  What is success criteria?
```
Based on the Candidate Onboarding Automation Project kickoff meeting transcript, the success criteria for the project are:

- 95% automation of onboarding steps
- <1 minute email trigger time
- 90% satisfaction in UAT feedback
- 40% reduction in onboarding duration

These success criteria were outlined by James (Project Manager) near the end of the kickoff meeting.
```

Verify the answers from the meeting transcripts. Once you are done asking questions, close the application. 