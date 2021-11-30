# Chalkboard

[Website Link - Deployed on Vercel](https://chalkboard-frontend.vercel.app/) 

[Backend Link - Deployed on Heroku](https://chalkboard-api.herokuapp.com/)
### Team Member: Sintheia Jerin Chowdhury


### Contribution: 




## Application Features

 -  Separete Login for Students and Instructors
 ```
 email: dummy1@email.com
 password: 0000
 ```
 - All Routes
 - Redirects are included incase of user is logged in or not.
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
For backend, we have used the nodejs and express while database is MongoDb.

[Backend can be find on this link](https://chalkboard-api.herokuapp.com/)

### User management
Their are two users in the web app, student and instructor. Both perform different actions due to their roll. So, both users will be managed differently
#### For Students

```

GET (all users) - https://chalkboard-api.herokuapp.com/users
GET (single user) - https://chalkboard-api.herokuapp.com/users/{user email}
POST - https://chalkboard-api.herokuapp.com/users/add_user
```
#### For Instructors

```
GET (all instructor) - https://chalkboard-api.herokuapp.com/instructors
GET (single instructor) - https://chalkboard-api.herokuapp.com/instructors/{user email}
POST - https://chalkboard-api.herokuapp.com/instructors/add
```
## Database Management System
For this project, we have used the MongoDb, noSQL Database.

### Students
We have implemented all the features, document required i.e first name, last name, email and password. But as student will carry more than that data. Student collection will contain the array of Enrolled Courses and Requested Courses which they requested for enrollement.
```
firstName : String,
lastName: String,
email : String,
password : String,
enrolledCourses: Array - reference from Courses and Instructors Model,
requestedCourses: Array - reference from Courses Model,
```

### Instructors
For instructor, we have added the same features as required and also the courses, instructor will teach, list of enrolled students and list of requested Courses
```
firstName : String,
lastName: String,
email : String,
password : String,
courses: Array - reference from Courses Model,
requestedCourses: Array - reference from Courses and Users Model,
enrolledStudents: Array - reference from Users Model
```


## Visual Design
[Link to Visual Designs](https://github.com/Stringbuilder101/chalkboard)

