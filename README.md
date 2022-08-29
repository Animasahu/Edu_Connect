# Edu_Connect
Edu Connect is all-in-one platform for e-learning. It is an easy-to-use and secure tool which helps teachers and students to connect and enrich the learning experiences together.

Website Link - <a href="https://educonnect-333219.web.app"> EduConnect </a> <br>
The website is hosted on a server that is owned by my college, and the frontend is hosted on Firebase.

How to get started with the website?
You can Sign up on the web application as students or teachers. However for teachers, their employee IDs are required. I have hard coded some values for employee IDs as of now, which you can find below.

Please use only these employee IDs while signing up as a teacher
![image](https://user-images.githubusercontent.com/70600260/187218052-2f5382d4-41fa-4fcc-9133-dcb363443956.png)

You can also find the same in a file named "EmployeeIDs" in the repository.

If you prefer logging in than signing up, here are a few credentials which might be helpful.

Login credentials - (checkout 'login credentials' file in the repo)

For student login, username = 'abhijitburman', password = 'Abhijit_1'

For teacher login, username = 'deepak' password = 'Deepak_1'

Once you login, you can explore the various features present in the website.

How to run the application locally?
Since the backend is already hosted, you may choose to only run the frontend locally. For doing so,

Clone the github repository.
Move to the directory of the project and do npm install
Run yarn start or npm start

![image](https://user-images.githubusercontent.com/70600260/187218224-fccb6d23-8f6b-434c-95dc-d86f5ca2683c.png)

In case you also want to run the backend locally, you need to

First create a database named "sample_db" in Postgresql.
Next, change the "BASE_URL" in 'src/config/routes.js' to 'http://localhost:3000/' (since now the requests would be made to localhost instead of the server the website is hosted on)
Create a '.env' file and paste the content of 'ENV' on this file.
Now open a new terminal (other than frontend) and chage directory to 'backend'.
Do npm install
Run nodemon index.js

![image](https://user-images.githubusercontent.com/70600260/187218365-239a4001-649a-48c5-a42c-3cbc8ebc97d8.png) <br>
You should be now able to run the application on localhost.

Technology Stack
Node.JS and Express.JS for backend
PostgreSQL for database
React for frontend
Hosted backend on a server owned by my college, and frontend on Firebase.

Database Design

![image](https://user-images.githubusercontent.com/70600260/187218527-9b7363c3-18d3-4a9d-a80f-2056bd0dedaf.png)

Main features of Edu Connect
Authentication System

User needs to sign up for using the features of this application. While doing so, one can sign up as a teacher or student as per their role. However, to prevent the students signing up as teachers, an "Employee ID" is required for the teachers.

Please note that,

organizations using this web application will also have to provide a list of Employee IDs for verification purposes.

![image](https://user-images.githubusercontent.com/70600260/187218673-3c7dca2d-38e1-4d19-8b43-363455cddce1.png)

Classes

As per the role of the user, the features of classes would be visible.

For a teacher, they will be allowed to create classrooms and schedule individual classes within them by providing the date and time.

![image](https://user-images.githubusercontent.com/70600260/187218816-5588390e-369e-423e-99bf-2e4549090a39.png)
![image](https://user-images.githubusercontent.com/70600260/187218900-b7cc9dd1-7783-4be5-89af-4b1f20f577a0.png)

For a student, they will only be allowed to join classes.

![image](https://user-images.githubusercontent.com/70600260/187218994-0a352b60-dd90-49e0-b772-feb428cc1e43.png)

Please note that,

to prevent any student joining any random class which they should not be a part of, a list of students who requested to join would be available to the teachers. Only after the teacher verifies, the student can join the particular class.
![image](https://user-images.githubusercontent.com/70600260/187219083-3d4c5913-b03d-4839-b4ff-74b1a9164346.png)

Book Offline Seats

While scheduling a class, the teacher needs to mention the number of offline seats available. Students will be able to book offline seats on first come first serve basis, based on the number of seats available.
![image](https://user-images.githubusercontent.com/70600260/187219178-56fd665c-4335-443c-bf61-032da2e47efc.png)

Upcoming Classes

Users can also view their upcoming classes in the coming days. The teachers would be able to see all the upcoming classes they have scheduled, and students would be able to view all the upcoming classes they are enrolled in.
![image](https://user-images.githubusercontent.com/70600260/187219251-ba948259-ab15-4792-9dd4-bf45a9faae23.png)

Video call

On starting any scheduled class by clicking 'START NOW', a video call gets started which the teacher and students can join to conduct classes.

![image](https://user-images.githubusercontent.com/70600260/187219352-ef2ccceb-47b8-4e33-bffc-cc0890f92ff3.png)

Assignments

Teachers on the website can upload and grade assignments, by viewing the submissions of the students.
![image](https://user-images.githubusercontent.com/70600260/187219448-523584cd-df44-4d4d-87bc-d57681ce6a07.png)

Students can filter the pending and completed assignments and submit their files on the website.
![image](https://user-images.githubusercontent.com/70600260/187219557-8234b4e4-4eaf-40d6-a9e3-aae074cfe8ab.png)

NOTE : Students and teachers both can upload pdf files not more than 5 MB in size.

Notifications

Teachers and students can communicate on the classroom using the notifications feature.

Future Scope
The notifications feature can be improved by adding a moderator, and the visuals can also be like a chat based application in the classroom.

A public forum feature can be added where students can ask their doubts and other students across all organizations can answer, with each question having tags and upvotes and downvotes for the answers.








