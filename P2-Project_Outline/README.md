# Project Outline
For this assignment, you will submit a high-level outline of your project. This can, and likely will, change over time. In particular, your mentor will provide feedback and direction and feedback to help sharpen your ideas. So don't worry if you feel unsure about some aspects of the outline, or if you have to change some things later.

## Assignment Description
[Project Outline Assignment](https://education.launchcode.org/liftoff/assignments/project-outline/)

## Submission Instructions

### Overview
The Grade-tracker app is a concept fullfilling a need in the homeschool and alternative school community for a dynamic record keeping application 
capable of tracking assignments, grades, and attendence. 
Homeschool comunities are limited in their ability to conveiniently and accurately tracking assignments and their associated grades. The state of the art software for grade and attendence tracking that had parnered with elements of the homeschool comunity is discontinuing their product, leaving this comunity in a deficite of grade-keeping software. To address this problem, I have proposed the construction of a low-cost / high yeild application. 
### Features
User login and Role Based Acess controlls:
This is the corner-stone of the application, as every student that logs in to the interface will see only their work and grades displayed, while 
the teachers that log in will only see their classes reflected in the display. 

Student Role: View only:
Once a student is logged in, he or she should see only a selection of the classes they are in, and their work displayed as well as the graded for that work (or lack therof).  

Teacher Role: add assignment, edit grade:
Once a teacher is logged in, they should be able to add an assignment to a certain class, and edit past assignments(including delete an assigment). 

Admin Role: Add students to a "co-op" Add classes, view grades,
There will be only one admin default for each "co-op", although if it isn't too time consuming I would like to have the capability of adding another admin to each "co-op".
Admins add students to the Co-op which creates a Student object that will coincide with a Student access account. On creation the Student will recieve a email prompt to login to their account.   
Teacher accounts are similar, with the only difference being a higher level access. 

Admins can add Classes, in order to do this they add a Class name, then select student names and a teacher name from a list. This will create a new Class object with a many-to-many relationship to the students and a has-a relationship to the teacher. 

Grading settings: 
Grading settings should be either predetermined, or they should be selected by the admin on creation of the class. these settings include grading catagories, school standards for letter grades, and possibly wieghted catagories. (I can see this section really going beyond the most basic necessary steps and becoming a liability). 

### Technologies
I need a technology with accessable role based access controls becasue that is the cornerstone of the application. 
I also need a front-end framework to display my views and in order to fill the recomendation of using a front end framework. 

I'm going to use Django because it has out-of-the-box capabilities in user account controlls / and role based access.
Becasue I'm using python I'll need to use a virtual enviroment. I will use Virtualenv for my virtual enviroment management. 
I am going to overlay a react-js framework onto the django back-end and templates.
For data persistance, I would like to use Firebase's cloud-based noSequel database, but I am willing to go to the old mysequel database if that doesn't work out so well. 


### What I'll Have to Learn
I will firstly need to learn to use react-js and become familiar with it's capabilities, in order to under stand the appropriate sharing of burdens/ layering for this project. 
I will then nead to finish learning how to use django to support my back-end requirements, which include advanced user acess controls and security. 
