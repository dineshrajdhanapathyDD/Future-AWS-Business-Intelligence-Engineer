## Submission

### List of Dataset Field names


- Create a New Sample Topic, using the  **Student Enrollment Statistics**  sample topic. This process will take several minutes.

<!-- <img width="1919" height="869" alt="Screenshot 2025-09-24 145838" src="https://github.com/user-attachments/assets/4a69858c-aee2-4b26-9fa2-0063ada211cf" /> -->

[![Screenshot-2025-09-24-145838.png](https://i.postimg.cc/1580cJrj/Screenshot-2025-09-24-145838.png)](https://postimg.cc/fJh0M7Fc)


Rename the  **HomeOfOrigin**  field to NationalOrigin, with a Description of: "Country of Residence on admission application"

<!-- <img width="1913" height="905" alt="Screenshot 2025-09-24 153147" src="https://github.com/user-attachments/assets/c954208d-76c0-4ecd-907a-cc022dbf0de3" /> -->

[![Screenshot-2025-09-24-153147.png](https://i.postimg.cc/QxZcL1L6/Screenshot-2025-09-24-153147.png)](https://postimg.cc/MXtnVcpR)

<!-- <img width="1918" height="935" alt="Screenshot 2025-09-24 153820" src="https://github.com/user-attachments/assets/75410515-efb6-480c-b32a-153b461395d8" /> -->

[![Screenshot-2025-09-24-153820.png](https://i.postimg.cc/6pm3Kx2t/Screenshot-2025-09-24-153820.png)](https://postimg.cc/RWw918LD)


### Dataset refresh schedule

- Configure the  **Q - Student Enrollment**  dataset with a Refresh schedule using the following settings:
- Timezone: Choose your local time zone
- Start time: Specify 12:00 AM on this coming Sunday
- Frequency: Weekly
- Refresh on: Sun

<!-- <img width="667" height="350" alt="Screenshot 2025-09-24 151232" src="https://github.com/user-attachments/assets/b4c69b6d-59f8-49e7-84e1-585433636eca" /> -->

[![Screenshot-2025-09-24-151232.png](https://i.postimg.cc/1RByP12j/Screenshot-2025-09-24-151232.png)](https://postimg.cc/Yjv5fZp6)


<!-- <img width="1919" height="697" alt="Screenshot 2025-09-24 151325" src="https://github.com/user-attachments/assets/86965351-1207-416a-9f15-72d2d09d6e76" /> -->

[![Screenshot-2025-09-24-151325.png](https://i.postimg.cc/yY54Y1Pj/Screenshot-2025-09-24-151325.png)](https://postimg.cc/XpwDs0tB)



### Student Type calculated field formula

- Add a calculated field to the dataset named  _Student Type_, using an ifelse function that returns "Youth" if {Age} is less than 30, and returns "Adult Continuing Education" for any other age.


<!-- <img width="1905" height="923" alt="Screenshot 2025-09-24 170305" src="https://github.com/user-attachments/assets/6a92f9a0-f407-49fd-80d0-bde656ea6901" /> -->

[![Screenshot-2025-09-24-170305.png](https://i.postimg.cc/6QfmRtrG/Screenshot-2025-09-24-170305.png)](https://postimg.cc/8Fs4g8n1)


### Each Visual in your analysis

- Create a new Analysis using the Q - Student Enrollment dataset. Add a new Visual to the Analysis using Q, using a prompt that asks for the the number of students in each major, grouped by their academic year. Edit the title of the new Visual to  _Student Majors by Year_. Resize the chart and legend areas to a comfortable size. Observe that Academic Year uses a comma to separate thousands. Change the format of the AcademicYear values to remove commas and other punctuation. Use the Edit with Q feature to reconfigure the Visual to use a vertical bar chart. Add a second visual to the Analysis, using a prompt that asks for a pie chart of the Student Types calculated field.Change the title of the Visual to  _Proportion of Student Types._ Resize the chart and legend areas to a comfortable size. Rename Sheet1 to  _Student Body Overview._

<!-- <img width="1918" height="939" alt="Screenshot 2025-09-24 164851" src="https://github.com/user-attachments/assets/da2f7b3a-827b-4022-8728-07fb4ebd7d26" /> -->

[![Screenshot-2025-09-24-164851.png](https://i.postimg.cc/jSbVJ8pP/Screenshot-2025-09-24-164851.png)](https://postimg.cc/6yYbkh5p)


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

    <!-- <img width="1908" height="917" alt="Screenshot 2025-09-24 170534" src="https://github.com/user-attachments/assets/6bc4d6f7-7969-4ece-baa4-7935acd85145" /> -->

    [![Screenshot-2025-09-24-170534.png](https://i.postimg.cc/KcMsrPDF/Screenshot-2025-09-24-170534.png)](https://postimg.cc/HjT2T7NP)
    
    - Entity Name 2: Course Details
    Field Ranking: Course, Professor, Cost per Course, Academic Year, Semester, Course Id

    <!-- <img width="1919" height="828" alt="Screenshot 2025-09-24 170723" src="https://github.com/user-attachments/assets/c291e196-638b-42b1-9aac-f3e406bee3e8" /> -->

    [![Screenshot-2025-09-24-170723.png](https://i.postimg.cc/qBsxvjxF/Screenshot-2025-09-24-170723.png)](https://postimg.cc/xqdzsG7G)
    
    - Entity Name 3: Professor Evaluation
    Field Ranking: Professor, Course, Semester, Academic Year, Student Name, Evaluation Score

    <!-- <img width="1919" height="843" alt="Screenshot 2025-09-24 170834" src="https://github.com/user-attachments/assets/6aa4e68f-4596-4daa-8c3f-4bc5af258fad" /> -->

    [![Screenshot-2025-09-24-170834.png](https://i.postimg.cc/qR0gbX6W/Screenshot-2025-09-24-170834.png)](https://postimg.cc/Z97T0NcL)


### The list of Verified answers in your topic


 Use the Open Q&A feature, and prompt Amazon Q to determine which instructors got the best average evaluations. Mark the answer as Verified

<!-- <img width="1272" height="846" alt="Screenshot 2025-09-24 170950" src="https://github.com/user-attachments/assets/62906419-5e79-4df0-8322-40942c5c976d" /> -->

[![Screenshot-2025-09-24-170950.png](https://i.postimg.cc/pLbvJVF7/Screenshot-2025-09-24-170950.png)](https://postimg.cc/gnD1YW4q)

<!-- <img width="1279" height="851" alt="Screenshot 2025-09-24 171001" src="https://github.com/user-attachments/assets/6ca5e488-328d-435c-b24a-2f3b719b6fd9" /> -->

[![Screenshot-2025-09-24-171001.png](https://i.postimg.cc/GhYtC5PP/Screenshot-2025-09-24-171001.png)](https://postimg.cc/hfDc8M5h)


- Prompt Amazon Q to determine which courses are the most expensive.
    - Does Amazon Q correctly understand the intent of your question? How do you know?

<!-- <img width="1278" height="847" alt="Screenshot 2025-09-24 171115" src="https://github.com/user-attachments/assets/99d6d63b-31bf-47ab-9c30-dcecc36aff26" /> -->

[![Screenshot-2025-09-24-171115.png](https://i.postimg.cc/RV0dpwwp/Screenshot-2025-09-24-171115.png)](https://postimg.cc/WtQ0hFW0)

- Correct Amazon Q's interpretation, if necessary.
    - Which courses are most expensive, on average?
 
<!-- <img width="1276" height="850" alt="Screenshot 2025-09-24 171223" src="https://github.com/user-attachments/assets/b2124e44-28cc-406c-9e43-a344d1f2c00c" />  -->

[![Screenshot-2025-09-24-171223.png](https://i.postimg.cc/CLdCsSgp/Screenshot-2025-09-24-171223.png)](https://postimg.cc/SJFzy0Rg)

- Mark the corrected answer as Verified.
    - Confirm your questions appear in the list of Verified questions.

<!-- <img width="1276" height="852" alt="Screenshot 2025-09-24 171232" src="https://github.com/user-attachments/assets/f500a1ed-69f0-4f1f-bf98-2d97442ac032" /> --> 

[![Screenshot-2025-09-24-171232.png](https://i.postimg.cc/KY5gyHbh/Screenshot-2025-09-24-171232.png)](https://postimg.cc/nsCL4TM3)

Select a few AI-Generated questions, and add their answers to the Verified list after ensuring that they produce useful results.

### Your Dashboard

- Create a dashboard by publishing the Q - Student Enrollment analysis as a new dashboard named  _Student Enrollment Dashboard_, in which data Q&A is allowed.


<!-- <img width="631" height="546" alt="Screenshot 2025-09-24 171556" src="https://github.com/user-attachments/assets/223d969c-3b2e-472a-beba-9f4e489b5711" /> -->

[![Screenshot-2025-09-24-171556.png](https://i.postimg.cc/ZqLyhMmZ/Screenshot-2025-09-24-171556.png)](https://postimg.cc/1gfzGM4Y)

- Test the Q&A feature of the dashboard by asking which Student Type has higher test scores.

<!-- <img width="1269" height="846" alt="Screenshot 2025-09-24 171809" src="https://github.com/user-attachments/assets/d362f518-f7ff-4e0f-999a-882463dbcf49" /> -->

[![Screenshot-2025-09-24-171809.png](https://i.postimg.cc/cJc8NbWd/Screenshot-2025-09-24-171809.png)](https://postimg.cc/XZpvfxXP)
 

- Extending an Analysis

    - Modify the  **Q - Student Enrollment**  Analysis, using Q to build four new visuals depicting the following:

    - Professors with the best average evaluations.

    <!-- <img width="1911" height="847" alt="Screenshot 2025-09-24 172654" src="https://github.com/user-attachments/assets/4c9d4781-a167-49d9-b1fb-9c5ade6ac9db" /> -->

    [![Screenshot-2025-09-24-172654.png](https://i.postimg.cc/6pqY1CxC/Screenshot-2025-09-24-172654.png)](https://postimg.cc/NKh6K9M0)

    - Courses with the best average evaluations.

    <!-- <img width="1918" height="932" alt="Screenshot 2025-09-24 172725" src="https://github.com/user-attachments/assets/97895ead-f269-4c18-952c-dfd8b5339220" /> -->

    [![Screenshot-2025-09-24-172725.png](https://i.postimg.cc/B6S8McRy/Screenshot-2025-09-24-172725.png)](https://postimg.cc/JyF4hJrc)
    

    - Professors with the highest average course costs.

    <!-- <img width="1919" height="939" alt="Screenshot 2025-09-24 172801" src="https://github.com/user-attachments/assets/d3eeeff4-6f4f-4d41-b57b-9364db59ae93" /> -->

    [![Screenshot-2025-09-24-172801.png](https://i.postimg.cc/zBvzydsV/Screenshot-2025-09-24-172801.png)](https://postimg.cc/34M56ZJT)

    - Courses with the highest average course costs.

    <!-- <img width="1919" height="930" alt="Screenshot 2025-09-24 172832" src="https://github.com/user-attachments/assets/913792c4-26aa-4725-8757-35e3bd1dff00" /> -->

    [![Screenshot-2025-09-24-172832.png](https://i.postimg.cc/wvn1g87b/Screenshot-2025-09-24-172832.png)](https://postimg.cc/MMb6mL0y)


    <!-- <img width="1917" height="931" alt="Screenshot 2025-09-24 173403" src="https://github.com/user-attachments/assets/ee44f1ef-f6db-43b6-8c6b-6ba24d3e3a6a" /> -->

    [![Screenshot-2025-09-24-173403.png](https://i.postimg.cc/1zjtrhcN/Screenshot-2025-09-24-173403.png)](https://postimg.cc/4KpsX00J)

    - Publish the Analysis, replacing the existing dashboard.

    <!-- <img width="540" height="514" alt="Screenshot 2025-09-24 173428" src="https://github.com/user-attachments/assets/b62a5964-bf8b-4eb1-bbcd-a1e98b1a8e76" /> -->


   [![Screenshot-2025-09-24-173428.png](https://i.postimg.cc/y8NsQpNg/Screenshot-2025-09-24-173428.png)](https://postimg.cc/Vd2x5Rnm)


### The starter question of your Scenario, and the follow-up questions in your Thread


- Create a new Scenario named,  _Improving Student Satisfaction Without Increasing Costs_ Select both Visuals from the Student Enrollment Dashboard as Data for this Scenario. 

<!-- <img width="1919" height="935" alt="Screenshot 2025-09-24 172309" src="https://github.com/user-attachments/assets/fbc8858a-2af8-425b-b13e-5d407b36a8ca" /> -->

[![Screenshot-2025-09-24-172309.png](https://i.postimg.cc/GmzJrtd8/Screenshot-2025-09-24-172309.png)](https://postimg.cc/MnMjmWcq)


- Start the Scenario with the question:  _How do we improve professor evaluations, while avoiding an increase in cost per course?_

<!-- <img width="1919" height="906" alt="Screenshot 2025-09-24 172525" src="https://github.com/user-attachments/assets/e7458af6-3371-4023-bc85-36b52243e07d" /> -->

[![Screenshot-2025-09-24-172525.png](https://i.postimg.cc/tCNFtJ1S/Screenshot-2025-09-24-172525.png)](https://postimg.cc/XpXZnVkd)


- Remove and recreate the  _Improving Student Satisfaction Without Increasing Costs_  scenario.
    - Select all Visuals from the Student Enrollment Dashboard as Data for this Scenario.

    <!-- <img width="1849" height="902" alt="Screenshot 2025-09-24 173533" src="https://github.com/user-attachments/assets/0c47518f-78c9-447c-8c8f-568f4e0d7deb" /> -->

     [![Screenshot-2025-09-24-173533.png](https://i.postimg.cc/kGcD8Vj4/Screenshot-2025-09-24-173533.png)](https://postimg.cc/JHs1ChCV)


    - Start the Scenario with the question:  _How do we improve professor evaluations, while avoiding an increase in cost per course?_

    <!-- <img width="1919" height="943" alt="Screenshot 2025-09-24 173919" src="https://github.com/user-attachments/assets/d3c95f31-0996-4f6b-9bfe-31085bf10dce" /> -->

    [![Screenshot-2025-09-24-173919.png](https://i.postimg.cc/fL7bntQk/Screenshot-2025-09-24-173919.png)](https://postimg.cc/LYXSjsXM)

    <!-- <img width="1918" height="898" alt="Screenshot 2025-09-24 174144" src="https://github.com/user-attachments/assets/247495c2-72a3-40b9-90f1-553f1750dede" /> -->

    [![Screenshot-2025-09-24-174144.png](https://i.postimg.cc/fyLQ2Jz3/Screenshot-2025-09-24-174144.png)](https://postimg.cc/YGJPj2mk)


- Start a thread with a prompt that attempts to determine what factors contribute to high professor evaluation scores.

    <!-- <img width="1919" height="913" alt="Screenshot 2025-09-24 174503" src="https://github.com/user-attachments/assets/3273a53d-c221-4676-9e15-014638770eaf" /> -->

    [![Screenshot-2025-09-24-174503.png](https://i.postimg.cc/FK9WgwsQ/Screenshot-2025-09-24-174503.png)](https://postimg.cc/DSMP7jXC)

    <!-- <img width="1919" height="937" alt="Screenshot 2025-09-24 174520" src="https://github.com/user-attachments/assets/963239fa-99da-4294-83e8-6b8e8a2d9a05" /> -->

    [![Screenshot-2025-09-24-174520.png](https://i.postimg.cc/mDnm4D3L/Screenshot-2025-09-24-174520.png)](https://postimg.cc/LYztBm0w)

    <!-- <img width="1915" height="916" alt="Screenshot 2025-09-24 174531" src="https://github.com/user-attachments/assets/959a2cab-0613-4a58-aa1a-ec1bb84c59a9" /> -->

    [![Screenshot-2025-09-24-174531.png](https://i.postimg.cc/wTXnXXcy/Screenshot-2025-09-24-174531.png)](https://postimg.cc/w7BWHsrg)

- Are you confident that you know what the college should do to improve student satisfaction while avoiding increasing costs? What are some other questions you could ask that could clarify the situation?

<!-- <img width="1917" height="934" alt="Screenshot 2025-09-24 174812" src="https://github.com/user-attachments/assets/870e2f0a-b092-4441-b1d7-89e210fad3f1" /> -->

[![Screenshot-2025-09-24-174812.png](https://i.postimg.cc/htMwwKYv/Screenshot-2025-09-24-174812.png)](https://postimg.cc/682Y4xtx)

<!-- <img width="1919" height="930" alt="Screenshot 2025-09-24 174838" src="https://github.com/user-attachments/assets/f6357ccd-6a99-44d7-93ee-ea3f76f12bc6" /> -->

[![Screenshot-2025-09-24-174838.png](https://i.postimg.cc/5NSkYxbq/Screenshot-2025-09-24-174838.png)](https://postimg.cc/N5LxZvy5)

<!-- <img width="1919" height="931" alt="Screenshot 2025-09-24 174936" src="https://github.com/user-attachments/assets/351756da-f749-4bbe-812c-31a8784950af" /> -->

[![Screenshot-2025-09-24-174936.png](https://i.postimg.cc/LsYTTRFJ/Screenshot-2025-09-24-174936.png)](https://postimg.cc/SX4CSBs4)

<!-- <img width="1919" height="938" alt="Screenshot 2025-09-24 175006" src="https://github.com/user-attachments/assets/e8bb981e-79c0-4de5-99bc-1197c51185e8" /> -->

[![Screenshot-2025-09-24-175006.png](https://i.postimg.cc/6q0L3pnj/Screenshot-2025-09-24-175006.png)](https://postimg.cc/m1PFpRdC)

- Add more questions to the scenario, perhaps supplementing the underlying analysis

<!-- <img width="1918" height="924" alt="Screenshot 2025-09-24 175525" src="https://github.com/user-attachments/assets/cf852727-135d-48d5-939a-021647d3c1a5" /> -->

[![Screenshot-2025-09-24-175525.png](https://i.postimg.cc/9MNcjGNw/Screenshot-2025-09-24-175525.png)](https://postimg.cc/vg9Jr6yG)


### complete Data Story


- Using Q, prompt to create a data story that demonstrates your student satisfaction improvement theory by including relevant visuals from the dashboard.

<!-- <img width="1919" height="796" alt="Screenshot 2025-09-24 183505" src="https://github.com/user-attachments/assets/12132574-26c0-49f1-9c04-71d66e044f93" /> -->

[![Screenshot-2025-09-24-183505.png](https://i.postimg.cc/KYGbk96t/Screenshot-2025-09-24-183505.png)](https://postimg.cc/YvsZTxqS)

<!-- <img width="1919" height="920" alt="Screenshot 2025-09-24 180137" src="https://github.com/user-attachments/assets/7ea1b5d9-2598-484f-bf45-a821f471cc31" /> -->

[![Screenshot-2025-09-24-180137.png](https://i.postimg.cc/kgc4pt9N/Screenshot-2025-09-24-180137.png)](https://postimg.cc/SnnkXRnj)

- Add visuals for Data stories

<!-- <img width="1919" height="926" alt="Screenshot 2025-09-24 181304" src="https://github.com/user-attachments/assets/cb6c0417-e483-4dc2-a045-d41af5b68154" /> -->

[![Screenshot-2025-09-24-181304.png](https://i.postimg.cc/bvwJcNwc/Screenshot-2025-09-24-181304.png)](https://postimg.cc/w1nHDzN0)

- Improve upon the AI data story output by adding text describing your own explanation of the data. Add additional text Blocks and Image blocks to emphasize your points.

- Edit the Story Cover area to add my name.

<!-- <img width="1915" height="934" alt="Screenshot 2025-09-24 183345" src="https://github.com/user-attachments/assets/f7b1176a-cca1-48eb-8209-fbd2ee1678b3" /> -->

[![Screenshot-2025-09-24-183345.png](https://i.postimg.cc/sgwjcd4R/Screenshot-2025-09-24-183345.png)](https://postimg.cc/75JrHRRB)


###   Listings of all created resources: Datasets, Analyses, Dashboards, Topics, Scenarios in this projects. 

<!-- <img width="1910" height="5765" alt="screencapture-us-west-2-quicksight-aws-amazon-sn-stories-648f5bca-c0a5-486c-b906-1188a7511586-edit-2025-09-24-18_29_45" src="https://github.com/user-attachments/assets/1ba02bd8-8c3e-4a5e-8a0a-879e8aeb768b" /> -->

[![screencapture-us-west-2-quicksight-aws-amazon-sn-stories-648f5bca-c0a5-486c-b906-1188a7511586-edit-2.png](https://i.postimg.cc/7YXrv1G0/screencapture-us-west-2-quicksight-aws-amazon-sn-stories-648f5bca-c0a5-486c-b906-1188a7511586-edit-2.png)](https://postimg.cc/7fCW02NZ)


<!-- <img width="1910" height="923" alt="screencapture-us-west-2-quicksight-aws-amazon-sn-account-UdacityQuicksightLab-analyses-bf0d81d1-d666-46fc-add6-698b4c596749-2025-09-24-18_37_45" src="https://github.com/user-attachments/assets/e4346025-5bf8-413f-a9f4-b7c594f26537" /> -->

[![screencapture-us-west-2-quicksight-aws-amazon-sn-account-Udacity-Quicksight-Lab-analyses-bf0d81d1-d666.png](https://i.postimg.cc/Cx1TwZk8/screencapture-us-west-2-quicksight-aws-amazon-sn-account-Udacity-Quicksight-Lab-analyses-bf0d81d1-d666.png)](https://postimg.cc/svt0cgnf)
