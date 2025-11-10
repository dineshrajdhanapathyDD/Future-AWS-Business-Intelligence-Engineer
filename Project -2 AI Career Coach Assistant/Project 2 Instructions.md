## Project Introduction

Career coaching at the fictitious Career4All involves skill-gap analysis and training recommendations, but the current manual process is inefficient and inconsistent. To address these challenges, this project focuses on building a web-based application using Amazon Q Apps. This no-code solution will automate skill-gap analysis by analyzing student CVs against job descriptions and recommending relevant training from Career4All’s digital catalog. Coaches will also be able to fine-tune recommendations using natural language inputs, ensuring consistency and up-to-date guidance for students.

## Project Summary

In this project, students will develop an AI-powered web application using Amazon Q Apps to support Career Coaches at Career4All. The application automates skill-gap analysis by comparing student CVs with job descriptions and generating personalized training recommendations from Career4All’s digital catalog. Coaches can refine these suggestions through natural language inputs, ensuring accuracy and consistency. By sharing the application across the coaching team, the project enhances efficiency, scalability, and the overall career guidance process.

# Environment Setup

### Learners will be using an AWS sandbox environment to complete this project.

### AWS Account and Access

-   Follow setup video to prepare the environment if needed.

## Downloading Course Files

-   Course-related files, such as  **sample CVs and job descriptions**, will be available for download from the  **learning interface**.


## Project Scenario: Automating Career Coaching

#### **Background**

Career4All, a leading career development platform, offers career coaching services to help learners align their skills with job opportunities. The organization's applications are hosted in the AWS cloud, and as a  **Cloud Engineer**, you are responsible for maintaining and optimizing these applications.

#### **Project Overview**

Your manager has assigned you a new task:  **assist Career Coaches in automating the Career Coaching process**  to improve efficiency and scalability. You recently had an initial discussion with  **Emma, the Lead Career Coach**, to better understand the challenges faced in the current process.

#### **Current Career Coaching Workflow**

1.  **Resume Review & Skill Gap Analysis**
    -   A career coach manually reviews the learner’s CV.
    -   The CV is compared against a job description to identify skill gaps.
2.  **Training Recommendations**
    -   Based on the skill-gap analysis, the coach selects relevant training programs from a catalog.
    -   A personalized learning schedule is created for the learner.
3.  **Customization of Recommendations**
    -   Coaches fine-tune recommendations based on factors such as:
        -   Learner’s current skill level
        -   Time availability
        -   Preferred learning format (videos, reading materials, hands-on labs, etc.)

#### **Key Challenges Identified**

-   **Manual & Time-Consuming Process**: The current workflow requires significant manual effort.
-   **Scalability Issues**: The number of learners seeking coaching has doubled in the last six months, making it difficult to keep up.
-   **Keeping Training Resources Updated**: Coaches struggle to stay up-to-date with evolving training programs and new technologies.

#### **Project Goal**

To develop an  **automated solution**  that streamlines the career coaching process, improves efficiency, and enables scalability, leveraging AWS services.

## Project Instructions

# High Level Instructions

## Section 1 – Setup Amazon Q Business

#### Project files can be found  [HERE(opens in a new tab)](https://github.com/udacity/CD14264-Building-Generative-AI-Apps-with-Amazon-Q-Business-Public)  or in the course download tab.

  

Watch this video to setup the environment for your project if needed.

https://www.youtube.com/watch?v=tIwYfgKbnH0


**Note**: If you use the Udacity provided Amazon Q Business, the following resources are pre-created for you:

-   Amazon Q Business application
    
-   IAM Identity center group
    
-   IAM Identity center users
    

![A screenshot of existing **CareerCoachAssistant** Q Business application](https://video.udacity-data.com/topher/2025/September/68b8651f_q/q.jpeg)

A screenshot of existing  **CareerCoachAssistant**  Q Business application

In Amazon Q Business in the AWS portal, select the application CareerCoachAssistant, click on "Admin Controls and Guardrails". Then click "Edit" under Global Controls. Make sure that "Allow end users to send queries directly to the LLM" is enabled and click "Save at the bottom right corner of page.

![A screenshot of existing **CareerCoaches group** in IAM Identity Center](https://video.udacity-data.com/topher/2025/September/68b58a98_9338d1d2-a174-43c5-bc59-3fd3a7373295/9338d1d2-a174-43c5-bc59-3fd3a7373295.jpeg)

A screenshot of existing  **CareerCoaches group**  in IAM Identity Center

## Section 2 – Create Application

  

Once the foundational setup of  **Amazon Q Business**  is complete, including configuring  **AWS IAM Identity Center**, setting up  **data sources**, and defining  **user access**, the next step is to  **create an application**.

We will follow a structured approach to  **build, enhance, and verify**  the application to ensure it meets business requirements efficiently.

Initially, we will  **create a simple application**  with minimal configurations. This helps establish a working foundation that can be progressively enhanced.

Once the basic application is set up, we will  **verify**  its functionality by accessing the web interface and performing test queries.

After validating the basic setup, we will  **expand the application's capabilities**  by integrating advanced features.

With each enhancement, we will conduct rigorous testing to confirm that the modifications align with expected functionality.

#### Task 1 – Setup a basic application

· Step 1.1 – Create a basic application

· Step 1.2 – Add input cards for CV and Job profile uploads

· Step 1.3 – Add output card for Skill gap analysis

· Step 1.4 – Add output card for training recommendation

· Step 1.5 – Verify the application

#### Task 2 – Customize the application

· Step 2.1 – Add output card for schedule

· Step 2.2 – Add input card for Recommendation by Coach

## Section 3 – Enhance your application

  

After successfully verifying the basic functionality of the application, a  **demo session was conducted for Career Coaches**  to showcase its capabilities. The feedback was overwhelmingly positive, with coaches appreciating the  **ease of use and intuitive interface**.

### Key Feedback from Career Coaches:

-   They find the application  **valuable and easy to navigate**.
-   They are eager to integrate it into their workflow.
-   During the discussion, they mentioned using a  **PDF course catalog**  as a  **reference**  when recommending training programs to learners.
-   They  **requested an option to include this PDF**  in the application as a  **data source**  so that Amazon Q Business can retrieve relevant information from it.

### Solution Exploration:

-   After exploring  **Amazon Q Business**, you discovered that  **document uploads**  can be included in the  **retrieval index**, making them searchable for queries.
-   The  **next step**  is to  **manually upload the PDF course catalog**  to be indexed and used within the application.

To  **enhance the application**  and  **meet the Career Coaches' request**, we will:

1.  **Manually upload the PDF course catalog**  into Amazon Q Business.
2.  **Ensure the document is indexed**, making its contents searchable.
3.  **Test the integration**  by querying the system to confirm it retrieves relevant course details.

#### Task 3 – Use the existing data source to query course catalog information

· Step 3.1 – Access the already uploaded PDF course catalog in Amazon Q Business.  
· Step 3.2 – Verify that your queries retrieve training recommendations from this source.  
· Step 3.3 – Confirm that results from the course catalog are integrated seamlessly with other data sources.

## Section 4 – Tap into additional course catalog

After demonstrating the ability to upload course catalog files manually, other Career Coaches were inspired and started sending additional static files containing course information. While this was a positive development, it quickly became apparent that manually uploading each file to Amazon Q Business was not scalable.

To overcome this challenge, you explored Amazon Q Business’s capability to use Amazon S3 as a data source. Instead of manually uploading documents one by one, you decided to:

· Create an Amazon S3 bucket in the same AWS region as your Amazon Q Business application.

· Allow Career Coaches to upload course catalog files directly to this bucket.

· Configure the S3 bucket as a data source in Amazon Q Business.

This approach will streamline document management, enable automatic syncing of new files, and ensure training recommendations stay up to date.

#### Task 4 – Add another data source

· Step 4.1 – Create an Amazon S3 bucket and upload static course catalog.

· Step 4.2 – Sync the data source.

· Step 4.3 – Verify that recommendations are including training from newly added source

· Step 4.4 – Setup a daily sync

## Section 5 – Enhance security of your application

  

A meeting was conducted with the  **Lead Coach**  to gather security and content moderation requirements for the training recommendation system. The discussion highlighted the need for  **access control**  based on coach expertise and  **content filtering**  to maintain the integrity of recommendations. The following key concerns were identified:

1.  **Restricted Course Access Based on Coach Expertise**
    -   Certain courses require  **specialized approval**  before being recommended.
    -   Coaches with expertise in  **specific fields**  (e.g.,  **Medicinal, Pediatric, Child Care**) should be the only ones allowed to recommend and view those courses.
    -   The system should  **dynamically filter recommendations**  based on the logged-in user’s qualifications.
2.  **Content Moderation and Keyword Blocking**
    -   The organization has identified a  **set of restricted words**  that must not appear in any training recommendations.
    -   Examples of blocked words include:  **Gambling, Casino, Self-harm, Attack**.
    -   The system should implement  **automatic filtering**  to remove any recommendations containing these keywords.

#### Task 5 – Restrict Course Access Based on Coach Expertise

· Step 5.1 – Use the existing  **CareerCoaches group**  in IAM Identity Center that has been set up in your account, allowing you to test access and recommendations as a Career Coach user.

· Step 5.2 – Upload restricted courses files to S3 bucket

· Step 5.3 – Create Access control list (ACL) configuration file and associate with the data source

#### Task 6 – Setup Keyword Blocking

· Step 6.1 – Block specific keywords.

## Section 6 – Share your application

#### Task 7 – Share your app

· Step 7.1 – Share your application with all users in the account.

## **Final state of the application**

![Architecture Diagram](https://video.udacity-data.com/topher/2025/April/67eeb82e_architecture/architecture.jpeg)

## Project Completion

We successfully automated the career coaching process for Career4All, transforming a manual and time-consuming workflow into an efficient, scalable system using AWS services. By leveraging Amazon Q Business, we developed an AI-powered solution that streamlines resume reviews, skill-gap analysis, and personalized training recommendations. The implementation included integrating dynamic data sources, such as Udacity and static course catalogs, and enabling seamless user interaction through a web-based application.

Additionally, we enhanced security by restricting course access based on coach expertise and implementing keyword filtering for content moderation. This project not only improved operational efficiency but also empowered Career Coaches with real-time, data-driven insights, allowing them to provide learners with up-to-date, tailored career guidance at scale.

## Submission of your project

**Include images of the following:**

### 1. Screenshot of your final application, showing all the input and output cards.

### 2. Screenshot of your data sources, showing the last sync time.

![Screenshot of your final application, showing all the input and output cards](https://video.udacity-data.com/topher/2025/June/685b3233_q1-final-application-screenshot/q1-final-application-screenshot.jpeg)

Screenshot of your final application, showing all the input and output cards.

### 3. Screenshot of the prompt you used for Skill Gap Analysis Output card.

![Screenshot of the prompt you used for Skill Gap Analysis Output card.](https://video.udacity-data.com/topher/2025/June/685b3347_q3-prompt/q3-prompt.jpeg)

Screenshot of the prompt you used for Skill Gap Analysis Output card.

### 4. Screenshot of the blocked words.

![Screenshot of the blocked words.](https://video.udacity-data.com/topher/2025/June/685b339c_q4-blocked-words/q4-blocked-words.jpeg)

Screenshot of the blocked words.

### 5. Upload the ACL file you created.

# Optional Additional Tasks (For advanced learners)

**Customize the Q App Web Experience (Theme / Logo / Text)**

Reference:  [https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/customizing-web-experience.html(opens in a new tab)](https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/customizing-web-experience.html)

**Automate Data Source sync using Amazon S3 event notification and AWS Lambda**

Reference:  [https://docs.aws.amazon.com/AmazonS3/latest/userguide/EventNotifications.html(opens in a new tab)](https://docs.aws.amazon.com/AmazonS3/latest/userguide/EventNotifications.html)

[https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/datasource-apis.html(opens in a new tab)](https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/datasource-apis.html)

**Connect your App to Microsoft Outlook to send recommendation emails and schedule reminders**

Reference:  [https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/integration-msoutlook.html(opens in a new tab)](https://docs.aws.amazon.com/amazonq/latest/qbusiness-ug/integration-msoutlook.html)

## Submission Instructions

Learners will be submitting the screenshots of a finished application interface, which should look like below image.

They can also submit the generated output in a PDF/Word document format after copying from Application.

![Application Interface](https://video.udacity-data.com/topher/2025/April/67eed190_final-application/final-application.jpeg)
