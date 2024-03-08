# Online-Examination-Web-Application
Online Examination Based Web Application.

Motivation for project
During COVID-19 pandemic it was very difficult for educational institution and private tuition to evaluate their student’s performance by taking examination, as lock-down was imposed in major part of the world. So, I had an Idea to build an application which will ease the process of evaluation based on examinations.

Implementation
The entire project is divided in to two major modules viz student and teacher each further divided into sub modules.

![image](https://github.com/devansh-akruvala/Online-Examination-Web-Application/assets/61865437/87fa3c87-146f-4b83-8924-83ad7b13984e)

Flow of Project.
My Work
I have implemented following modules of the project:-

1. Student side login and signup module

2. Student side homepage module

3. Student side give exam module

4. Student side view result module

Database Schema

Studentdetails(name, semail, dept, college, password)

Teacherdetails(name, email , dept, college, password)

Questionbank(eid, option1, option2, option3, option4, ans)

Examdetails(temail, eid, subject, syllabus, date_time, timelimit)

Result(email, eid, marks)

Login and Signup module
This module consist of login and signup form, form validation, user verification by mail. On completing verification data of new user is added into database.


Login page.<br>

![image](https://github.com/devansh-akruvala/Online-Examination-Web-Application/assets/61865437/af87717b-760d-4eb4-88f1-31ea061f40ba)

Signup Page.<br>
![image](https://github.com/devansh-akruvala/Online-Examination-Web-Application/assets/61865437/8e42f6ef-9aa1-4e1b-a403-9cb3a8b854b0)

verification link is send to users email id and after clicking the link all the entered data is stored in database.

![image](https://github.com/devansh-akruvala/Online-Examination-Web-Application/assets/61865437/a16467c7-1b82-47ca-90a0-c12af898102e)

Verification mail link on user email.

![image](https://github.com/devansh-akruvala/Online-Examination-Web-Application/assets/61865437/eaa17032-9bb1-4514-b405-43c143fbb582)

After verification data is stored in database.
<br>
<br>
This module contains additional sub module called forgot password. If user forgets his/her password then he can reset his password. A link is send to register email from which he/she can reset his password.

![image](https://github.com/devansh-akruvala/Online-Examination-Web-Application/assets/61865437/11593616-954d-4ac4-91ed-e8e611017a19)

Password Reset link.
2. Student side Homepage Module

After entering correct login credential user is redirected to home page. This page contains all the upcoming exams detail. Student have to enter exam id code provided by teacher and all the information like subject syllabus date and time of exam etc will be displayed. all the details is fetched form Examdetails table.

Student Home page.<br>
![image](https://github.com/devansh-akruvala/Online-Examination-Web-Application/assets/61865437/06eb340b-dc44-4977-b1e5-8734a98c22b3)


All the details like subject, syllabus, date and time, time limit are fetched from the Questionbank table corresponding to entered “eid” and displayed as a card view with help of tool called repeater. On clicking on specific exam Date and time of system is compared with assigned date and time in database and content are displayed within assigned time.


Data of Examdetails table.<br>
![image](https://github.com/devansh-akruvala/Online-Examination-Web-Application/assets/61865437/d2125749-24b9-4084-a278-6b0781b334f1)


3. Exam Giving module

This is the heart of this application. It have numerous amount of features like exam can only be opened on specified date and time, Fetching all questions from database. Evaluating answers on click of submit button and storing result in database. Answer should be submitted within specified time limit.


Exam giving module.<br>
![image](https://github.com/devansh-akruvala/Online-Examination-Web-Application/assets/61865437/c0629c99-3a51-4a18-9733-f1da87e16bb3)

All Question are fetched from Questionbank table with help of entered “eid” value, correct answer and user answer is compared and score is calculated accordingly.


Data of Questionbank table.<br>
![image](https://github.com/devansh-akruvala/Online-Examination-Web-Application/assets/61865437/176a1475-5252-434c-aed5-ffb2975f7e79)

4. Student side Result module

This module shows marks of all the past examination and is used to keep track of result in all subjects. It fetches all info from data base corresponding to users email id and shows in form of table.


Student Side Result page.<br>
![image](https://github.com/devansh-akruvala/Online-Examination-Web-Application/assets/61865437/95954678-4c1f-40b1-b335-173d5766ce6c)

## Video
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/Dih-jZbsTiM/0.jpg)](https://www.youtube.com/watch?v=Dih-jZbsTiM)
