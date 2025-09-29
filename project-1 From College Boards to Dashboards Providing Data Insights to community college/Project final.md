## Submission

### List of Dataset Field names


- Create a New Sample Topic, using the  **Student Enrollment Statistics**  sample topic. This process will take several minutes.

<img width="1919" height="869" alt="Screenshot 2025-09-24 145838" src="https://github.com/user-attachments/assets/4a69858c-aee2-4b26-9fa2-0063ada211cf" />

Rename the  **HomeOfOrigin**  field to NationalOrigin, with a Description of: "Country of Residence on admission application"

<img width="1913" height="905" alt="Screenshot 2025-09-24 153147" src="https://github.com/user-attachments/assets/c954208d-76c0-4ecd-907a-cc022dbf0de3" />



<img width="1918" height="935" alt="Screenshot 2025-09-24 153820" src="https://github.com/user-attachments/assets/75410515-efb6-480c-b32a-153b461395d8" />


### Dataset refresh schedule

- Configure the  **Q - Student Enrollment**  dataset with a Refresh schedule using the following settings:
- Timezone: Choose your local time zone
- Start time: Specify 12:00 AM on this coming Sunday
- Frequency: Weekly
- Refresh on: Sun

<img width="667" height="350" alt="Screenshot 2025-09-24 151232" src="https://github.com/user-attachments/assets/b4c69b6d-59f8-49e7-84e1-585433636eca" />


<img width="1919" height="697" alt="Screenshot 2025-09-24 151325" src="https://github.com/user-attachments/assets/86965351-1207-416a-9f15-72d2d09d6e76" />



### Student Type calculated field formula

- Add a calculated field to the dataset named  _Student Type_, using an ifelse function that returns "Youth" if {Age} is less than 30, and returns "Adult Continuing Education" for any other age.


<img width="1905" height="923" alt="Screenshot 2025-09-24 170305" src="https://github.com/user-attachments/assets/6a92f9a0-f407-49fd-80d0-bde656ea6901" />


### Each Visual in your analysis

- Create a new Analysis using the Q - Student Enrollment dataset. Add a new Visual to the Analysis using Q, using a prompt that asks for the the number of students in each major, grouped by their academic year. Edit the title of the new Visual to  _Student Majors by Year_. Resize the chart and legend areas to a comfortable size. Observe that Academic Year uses a comma to separate thousands. Change the format of the AcademicYear values to remove commas and other punctuation. Use the Edit with Q feature to reconfigure the Visual to use a vertical bar chart. Add a second visual to the Analysis, using a prompt that asks for a pie chart of the Student Types calculated field.Change the title of the Visual to  _Proportion of Student Types._ Resize the chart and legend areas to a comfortable size. Rename Sheet1 to  _Student Body Overview._

<img width="1918" height="939" alt="Screenshot 2025-09-24 164851" src="https://github.com/user-attachments/assets/da2f7b3a-827b-4022-8728-07fb4ebd7d26" />


### Each Named Entity in your topic

- Create a new Topic using the following information:
    - Topic Name: Regional Community College Student Data
    - Description: Q&A environment for understanding student enrollment data Wait while setup completes. This process will take several minutes.
- Include the following Data Fields in this Topic:
    - Student Type, NationalOrigin, Gender, StudentClassification, Course, Grade, TestScore, Semester, CourseId, Professor, Credit, CostPerCourse, EvaluationScore, StudentName, StudentId, AcademicYear, EnrollmentDate, GraduationDate, Major, Age.
  
- Create 3 Named Entities inside the Topic, using the following details:
    - Entity Name 1: Student Details
    Description: Information about enrolled students
    Field Ranking: Student Name, Semester, Course, Test Score, Grade, Student Classification, Student Type, Major, Gender, NationalOrigin, Credit, Enrollment Date, Graduation Date, Student Id

    <img width="1908" height="917" alt="Screenshot 2025-09-24 170534" src="https://github.com/user-attachments/assets/6bc4d6f7-7969-4ece-baa4-7935acd85145" />
    
    - Entity Name 2: Course Details
    Field Ranking: Course, Professor, Cost per Course, Academic Year, Semester, Course Id

    <img width="1919" height="828" alt="Screenshot 2025-09-24 170723" src="https://github.com/user-attachments/assets/c291e196-638b-42b1-9aac-f3e406bee3e8" />
    
    - Entity Name 3: Professor Evaluation
    Field Ranking: Professor, Course, Semester, Academic Year, Student Name, Evaluation Score

    <img width="1919" height="843" alt="Screenshot 2025-09-24 170834" src="https://github.com/user-attachments/assets/6aa4e68f-4596-4daa-8c3f-4bc5af258fad" />


### The list of Verified answers in your topic


 Use the Open Q&A feature, and prompt Amazon Q to determine which instructors got the best average evaluations. Mark the answer as Verified

<img width="1272" height="846" alt="Screenshot 2025-09-24 170950" src="https://github.com/user-attachments/assets/62906419-5e79-4df0-8322-40942c5c976d" />

<img width="1279" height="851" alt="Screenshot 2025-09-24 171001" src="https://github.com/user-attachments/assets/6ca5e488-328d-435c-b24a-2f3b719b6fd9" />



- Prompt Amazon Q to determine which courses are the most expensive.
    - Does Amazon Q correctly understand the intent of your question? How do you know?

<img width="1278" height="847" alt="Screenshot 2025-09-24 171115" src="https://github.com/user-attachments/assets/99d6d63b-31bf-47ab-9c30-dcecc36aff26" />

- Correct Amazon Q's interpretation, if necessary.
    - Which courses are most expensive, on average?
 
<img width="1276" height="850" alt="Screenshot 2025-09-24 171223" src="https://github.com/user-attachments/assets/b2124e44-28cc-406c-9e43-a344d1f2c00c" /> 

- Mark the corrected answer as Verified.
    - Confirm your questions appear in the list of Verified questions.

<img width="1276" height="852" alt="Screenshot 2025-09-24 171232" src="https://github.com/user-attachments/assets/f500a1ed-69f0-4f1f-bf98-2d97442ac032" />  

Select a few AI-Generated questions, and add their answers to the Verified list after ensuring that they produce useful results.

### Your Dashboard

- Create a dashboard by publishing the Q - Student Enrollment analysis as a new dashboard named  _Student Enrollment Dashboard_, in which data Q&A is allowed.


<img width="631" height="546" alt="Screenshot 2025-09-24 171556" src="https://github.com/user-attachments/assets/223d969c-3b2e-472a-beba-9f4e489b5711" /> 

- Test the Q&A feature of the dashboard by asking which Student Type has higher test scores.

<img width="1269" height="846" alt="Screenshot 2025-09-24 171809" src="https://github.com/user-attachments/assets/d362f518-f7ff-4e0f-999a-882463dbcf49" />


- Extending an Analysis

    - Modify the  **Q - Student Enrollment**  Analysis, using Q to build four new visuals depicting the following:

    - Professors with the best average evaluations.

    <img width="1911" height="847" alt="Screenshot 2025-09-24 172654" src="https://github.com/user-attachments/assets/4c9d4781-a167-49d9-b1fb-9c5ade6ac9db" />

    - Courses with the best average evaluations.

    <img width="1918" height="932" alt="Screenshot 2025-09-24 172725" src="https://github.com/user-attachments/assets/97895ead-f269-4c18-952c-dfd8b5339220" />

    - Professors with the highest average course costs.

    <img width="1919" height="939" alt="Screenshot 2025-09-24 172801" src="https://github.com/user-attachments/assets/d3eeeff4-6f4f-4d41-b57b-9364db59ae93" />

    - Courses with the highest average course costs.

    <img width="1919" height="930" alt="Screenshot 2025-09-24 172832" src="https://github.com/user-attachments/assets/913792c4-26aa-4725-8757-35e3bd1dff00" />


    <img width="1917" height="931" alt="Screenshot 2025-09-24 173403" src="https://github.com/user-attachments/assets/ee44f1ef-f6db-43b6-8c6b-6ba24d3e3a6a" />

    - Publish the Analysis, replacing the existing dashboard.

    <img width="540" height="514" alt="Screenshot 2025-09-24 173428" src="https://github.com/user-attachments/assets/b62a5964-bf8b-4eb1-bbcd-a1e98b1a8e76" />


   




### The starter question of your Scenario, and the follow-up questions in your Thread


- Create a new Scenario named,  _Improving Student Satisfaction Without Increasing Costs_ Select both Visuals from the Student Enrollment Dashboard as Data for this Scenario. 
<img width="1919" height="935" alt="Screenshot 2025-09-24 172309" src="https://github.com/user-attachments/assets/fbc8858a-2af8-425b-b13e-5d407b36a8ca" />


- Start the Scenario with the question:  _How do we improve professor evaluations, while avoiding an increase in cost per course?_

<img width="1919" height="906" alt="Screenshot 2025-09-24 172525" src="https://github.com/user-attachments/assets/e7458af6-3371-4023-bc85-36b52243e07d" />


- Remove and recreate the  _Improving Student Satisfaction Without Increasing Costs_  scenario.
    - Select all Visuals from the Student Enrollment Dashboard as Data for this Scenario.

     <img width="1849" height="902" alt="Screenshot 2025-09-24 173533" src="https://github.com/user-attachments/assets/0c47518f-78c9-447c-8c8f-568f4e0d7deb" />


    - Start the Scenario with the question:  _How do we improve professor evaluations, while avoiding an increase in cost per course?_

    <img width="1919" height="943" alt="Screenshot 2025-09-24 173919" src="https://github.com/user-attachments/assets/d3c95f31-0996-4f6b-9bfe-31085bf10dce" />

    <img width="1918" height="898" alt="Screenshot 2025-09-24 174144" src="https://github.com/user-attachments/assets/247495c2-72a3-40b9-90f1-553f1750dede" />


    


- Start a thread with a prompt that attempts to determine what factors contribute to high professor evaluation scores.

    <img width="1919" height="913" alt="Screenshot 2025-09-24 174503" src="https://github.com/user-attachments/assets/3273a53d-c221-4676-9e15-014638770eaf" />

    <img width="1919" height="937" alt="Screenshot 2025-09-24 174520" src="https://github.com/user-attachments/assets/963239fa-99da-4294-83e8-6b8e8a2d9a05" />

    <img width="1915" height="916" alt="Screenshot 2025-09-24 174531" src="https://github.com/user-attachments/assets/959a2cab-0613-4a58-aa1a-ec1bb84c59a9" />

- Are you confident that you know what the college should do to improve student satisfaction while avoiding increasing costs? What are some other questions you could ask that could clarify the situation?

<img width="1917" height="934" alt="Screenshot 2025-09-24 174812" src="https://github.com/user-attachments/assets/870e2f0a-b092-4441-b1d7-89e210fad3f1" />

<img width="1919" height="930" alt="Screenshot 2025-09-24 174838" src="https://github.com/user-attachments/assets/f6357ccd-6a99-44d7-93ee-ea3f76f12bc6" />

<img width="1919" height="931" alt="Screenshot 2025-09-24 174936" src="https://github.com/user-attachments/assets/351756da-f749-4bbe-812c-31a8784950af" />

<img width="1919" height="938" alt="Screenshot 2025-09-24 175006" src="https://github.com/user-attachments/assets/e8bb981e-79c0-4de5-99bc-1197c51185e8" />

- Add more questions to the scenario, perhaps supplementing the underlying analysis

<img width="1918" height="924" alt="Screenshot 2025-09-24 175525" src="https://github.com/user-attachments/assets/cf852727-135d-48d5-939a-021647d3c1a5" />


### complete Data Story


- Using Q, prompt to create a data story that demonstrates your student satisfaction improvement theory by including relevant visuals from the dashboard.

<img width="1919" height="796" alt="Screenshot 2025-09-24 183505" src="https://github.com/user-attachments/assets/12132574-26c0-49f1-9c04-71d66e044f93" />

<img width="1919" height="920" alt="Screenshot 2025-09-24 180137" src="https://github.com/user-attachments/assets/7ea1b5d9-2598-484f-bf45-a821f471cc31" />

- Add visuals for Data stories

<img width="1919" height="926" alt="Screenshot 2025-09-24 181304" src="https://github.com/user-attachments/assets/cb6c0417-e483-4dc2-a045-d41af5b68154" />

- Improve upon the AI data story output by adding text describing your own explanation of the data. Add additional text Blocks and Image blocks to emphasize your points.

- Edit the Story Cover area to add my name.

<img width="1915" height="934" alt="Screenshot 2025-09-24 183345" src="https://github.com/user-attachments/assets/f7b1176a-cca1-48eb-8209-fbd2ee1678b3" />





###   Listings of all created resources: Datasets, Analyses, Dashboards, Topics, Scenarios in this projects. 

<img width="1910" height="5765" alt="screencapture-us-west-2-quicksight-aws-amazon-sn-stories-648f5bca-c0a5-486c-b906-1188a7511586-edit-2025-09-24-18_29_45" src="https://github.com/user-attachments/assets/1ba02bd8-8c3e-4a5e-8a0a-879e8aeb768b" />


<img width="1910" height="923" alt="screencapture-us-west-2-quicksight-aws-amazon-sn-account-UdacityQuicksightLab-analyses-bf0d81d1-d666-46fc-add6-698b4c596749-2025-09-24-18_37_45" src="https://github.com/user-attachments/assets/e4346025-5bf8-413f-a9f4-b7c594f26537" />

