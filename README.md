# Chalkboard

[Website Link](https://webapp-eosin.vercel.app/)

### Team Member: Sintheia Jerin Chowdhury


### Contribution: 




## Application Features

 -  Separete Login for Students and Instructors
 ```
 email: dummy1@email.com
 password: 0000
 ```
 - All Routes
 ```
 / (Home Page)
 /browse (Browse Courses Screen)
 /browse/:id (Course Screen after clicking any of course)
 /login (Select Login for student or instructor)
 /login/student (Login as a student)
 /login/instructor (Login as instructor)
 /:userId/dashboard (User will be redirected here after logging in to student)
 /:user/instructor/dashboard (User will be redirected here after logging in to instructor)
 /:user/dashboard/assignments (Assignments Page)
 /:user/assignments/:assignmentId (User can see course assignment if logged In) 
 
 ```
 `/login/student` for student
 `/login/instructor` for instructors
 - Instructor Dashboard with information related to total enrolled students and course instructing 
 `/instructor/dashboard` (You need to login first on instructor page)
 
 - Student Dashboard with information related to enrolled courses and requested for enrollement
 `/:userId/dashboard`
 - Users can view all their assignments by going to link attached in sidebar
 `/:userId/assignments`
 - Users can go to the course and view separate assignments related to course
  `/browse/:courseId/`  (if enrolled - todo)
 - Users can attempt to solve the assignment questions or upload the image or pdf file as answer. User can submit or save as draft
 `/assignments/:assignmentId`


## Frontend Technologies 
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/React-icon.svg/512px-React-icon.svg.png" alt="drawing" width="200"/>

React js is a frontend javaScript Library developed by Facebook.

## Backend Technologies
yet to decide

## Database Management System
yet to decide

## Visual Design
[Link to Visual Designs](https://github.com/Stringbuilder101/chalkboard)

