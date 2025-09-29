## Project Instructions

### Create and Prepare the College Dataset in Amazon QuickSight

1.  Attempt to create a new Dataset using the following details.


    1.  Data source name: Regional Community College Student Enrollment Data
    2.  Manifest file: s3://RegionalCommunityCollegeBucket/EnrollmentData/EnrollmentManifest.json
2.  Observe the error, and cancel dataset creation. The provided S3 bucket name is fictional and is not part of this project.
3.  Create a New Sample Topic, using the  **Student Enrollment Statistics**  sample topic. This process will take several minutes.
4.  Configure the  **Q - Student Enrollment**  dataset with a Refresh schedule using the following settings:
5.  Timezone: Choose your local time zone
6.  Start time: Specify 12:00 AM on this coming Sunday
7.  Frequency: Weekly
8.  Refresh on: Sun
9.  Configure the permissions of the Q - Student Enrollment dataset to add  _[admissions@regionalcommunity.edu(opens in a new tab)](mailto:admissions@regionalcommunity.edu)_  as a user of the dataset.

_Observe the error message. This email address is fictional , not part of this project, and can not be added._

6.  Rename the  **HomeOfOrigin**  field to NationalOrigin, with a Description of: "Country of Residence on admission application"
7.  Add a calculated field to the dataset named  _Student Type_, using an ifelse function that returns "Youth" if {Age} is less than 30, and returns "Adult Continuing Education" for any other age.
8.  Save & Publish the Dataset.

### Create an Analysis of the Dataset using Q

1.  Create a new Analysis using the Q - Student Enrollment dataset.
2.  Add a new Visual to the Analysis using Q, using a prompt that asks for the the number of students in each major, grouped by their academic year.
3.  Consider: What do you like about the new visual? What elements of it would you change to make it easier for a viewer to understand?
4.  Edit the title of the new Visual to  _Student Majors by Year_
5.  Resize the chart and legend areas to a comfortable size.
6.  Observe that Academic Year uses a comma to separate thousands.
7.  Change the format of the AcademicYear values to remove commas and other punctuation.
8.  Use the Edit with Q feature to reconfigure the Visual to use a vertical bar chart.
9.  Add a second visual to the Analysis, using a prompt that asks for a pie chart of the Student Types calculated field.
10.  Change the title of the Visual to  _Proportion of Student Types._
11.  Resize the chart and legend areas to a comfortable size.
12.  Rename Sheet1 to  _Student Body Overview._

### Configuring a Q Topic

1.  Delete the provided  **Student Enrollment (Sample)**  topic.
2.  Create a new Topic using the following information:
3.  Topic Name: Regional Community College Student Data
4.  Description: Q&A environment for understanding student enrollment data
5.  Wait while setup completes. This process will take several minutes.
6.  Include the following Data Fields in this Topic:
7.  Student Type, NationalOrigin, Gender, StudentClassification, Course, Grade, TestScore, Semester, CourseId, Professor, Credit, CostPerCourse, EvaluationScore, StudentName, StudentId, AcademicYear, EnrollmentDate, GraduationDate, Major, Age.
8.  Create 3 Named Entities inside the Topic, using the following details:
9.  Entity Name 1: Student Details
10.  Description: Information about enrolled students
11.  Field Ranking: Student Name, Semester, Course, Test Score, Grade, Student Classification, Student Type, Major, Gender, NationalOrigin, Credit, Enrollment Date, Graduation Date, Student Id
12.  Entity Name 2: Course Details
13.  Field Ranking: Course, Professor, Cost per Course, Academic Year, Semester, Course Id
14.  Entity Name 3: Professor Evaluation
15.  Field Ranking: Professor, Course, Semester, Academic Year, Student Name, Evaluation Score
16.  Use the Open Q&A feature, and prompt Amazon Q to determine which instructors got the best average evaluations.
17.  Mark the answer as Verified
18.  Prompt Amazon Q to determine which courses are the most expensive.
19.  Consider: Does Amazon Q correctly understand the intent of your question? How do you know?
20.  Correct Amazon Q's interpretation, if necessary.
21.  Consider: Which courses are most expensive, on average?
22.  Mark the corrected answer as Verified.
23.  Confirm your questions appear in the list of Verified questions.
24.  Select a few AI-Generated questions, and add their answers to the Verified list after ensuring that they produce useful results.

### Creating Dashboards

1.  Create a dashboard by publishing the Q - Student Enrollment analysis as a new dashboard named  _Student Enrollment Dashboard_, in which data Q&A is allowed.
2.  Test the Q&A feature of the dashboard by asking which Student Type has higher test scores.

### Creating Scenarios

1.  Create a new Scenario named,  _Improving Student Satisfaction Without Increasing Costs_
2.  Select both Visuals from the Student Enrollment Dashboard as Data for this Scenario.
3.  Start the Scenario with the question:  _How do we improve professor evaluations, while avoiding an increase in cost per course?_

Consider: Do the offered starter questions provide a satisfying start to answering this business question? Why do you think that is? What would make this Scenario more useful?

### Extending an Analysis

1.  Modify the  **Q - Student Enrollment**  Analysis, using Q to build four new visuals depicting the following:
2.  Professors with the best average evaluations.
3.  Courses with the best average evaluations.
4.  Professors with the highest average course costs.
5.  Courses with the highest average course costs.
6.  Publish the Analysis, replacing the existing dashboard.

### Developing a Scenario

1.  Remove and recreate the  _Improving Student Satisfaction Without Increasing Costs_  scenario.
2.  Select all Visuals from the Student Enrollment Dashboard as Data for this Scenario.
3.  Start the Scenario with the question:  _How do we improve professor evaluations, while avoiding an increase in cost per course?_
4.  Consider: Are the suggested questions an improvement over the original list? Are there other elements you would like to add to the Analysis and Dashboard?
5.  Start a thread with a prompt that attempts to determine what factors contribute to high professor evaluation scores.
6.  Consider: Are you confident that you know what the college should do to improve student satisfaction while avoiding increasing costs? What are some other questions you could ask that could clarify the situation?
7.  Add more questions to the scenario, perhaps supplementing the underlying analysis, until you arrive at a recommendation to bring to the college's board of directors.

### Create a Data Story

1.  Using Q, prompt to create a data story that demonstrates your student satisfaction improvement theory by including relevant visuals from the dashboard.
2.  Consider: Does the AI-generated story provide a satisfying explanation of your theory? What should be added? Do you need to supplement or recreate your analysis or dashboard? Data analysis projects often require an iterative approach to get to results that are of use to the organization. Don't be surprised if it takes multiple attempts to get the results you want.
3.  Improve upon the AI data story output by adding text describing your own explanation of the data. Add additional text Blocks and Image blocks to emphasize your points.
4.  Use the Story Style button to change the story style to one of your liking.
5.  Edit the Story Cover area to add your name.

## Submission Instructions

Use your computer's screenshot capability to capture a visual record of all elements of your work in a word processor document for submission. Please label screenshot images for reference by your mentor.

Your submission should include:

-   List of Dataset Field names
-   Dataset refresh schedule
-   Student Type calculated field formula
-   Each Visual in your analysis
-   Each Named Entity in your topic
-   The list of Verified answers in your topic
-   Your Dashboard
-   The starter question of your Scenario, and the follow-up questions in your Thread
-   Your complete Data Story
-   Listings of all created resources: Datasets, Analyses, Dashboards, Topics, Scenarios

