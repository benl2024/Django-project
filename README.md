
# Online Course Management System

This is an Online Course Management System that allows users to register, enroll in courses, take exams, and view their exam results.

## ER Diagram

The ER diagram below illustrates the database schema used in the Online Course Web Application. It outlines the entities and their relationships, providing an overview of how data is structured within the application.

![Onlinecourse ER Diagram](https://github.com/ibm-developer-skills-network/final-cloud-app-with-database/blob/master/static/media/course_images/onlinecourse_app_er.png)

The main entities in the diagram include:

- Course: Represents a course offered on the platform, containing details such as course name, description, and enrollment information.

- Lesson: Corresponds to individual lessons or topics within a course. Lessons are associated with their respective courses.

- Exam: Represents an exam associated with a course. Exams consist of multiple-choice questions.

- User: Represents a user of the application, whether it's a student or an instructor.

- Enrollment: Tracks the enrollment status of users in specific courses.

The ER diagram serves as a visual representation of the underlying database structure, facilitating a better understanding of how the application manages and organizes course-related data.

## Features

1. User Registration and Login
   - Users can register for an account and log in using their credentials.

2. Course Listing and Details
   - Users can view a list of available courses and see the details of each course.

3. Course Enrollment
   - Users can enroll in courses they are interested in.

4. Taking Exams
   - Enrolled users can take exams for the courses they are enrolled in.

5. Viewing Exam Results
   - After taking an exam, users can view their exam results and see which questions they answered correctly and incorrectly.

## Setup Instructions

1. Clone the Repository
```
git clone https://github.com/your-username/online-course-management.git
cd online-course-management
```
2. Install Dependencies
```
pip install -r requirements.txt
```
3. Set Up the Database

- Create a new database in your preferred database management system (e.g., PostgreSQL, MySQL).
- Update the database settings in `settings.py` to point to your database.

4. Run Migrations
```
python manage.py makemigrations
python manage.py migrate
```
5. Create a Superuser

- Create a superuser account to access the admin interface.
```
python manage.py createsuperuser
```
7. Access the Application

- Open your web browser and go to `http://localhost:8000/` to access the application.
- Use the superuser account to log in to the admin interface at `http://localhost:8000/admin/`.

## Usage Instructions

1. Registration and Login

- Users can register for a new account or log in using their existing credentials.
- New users need to fill out the registration form with their username, first name, last name, and password.

2. Course Listing and Enrollment

- After logging in, users can view a list of available courses.
- Users can click on a course to view its details and enroll in the course if they are interested.

3. Taking Exams

- Enrolled users can take exams for the courses they are enrolled in.
- Each exam consists of multiple-choice questions with several choices.
- Users need to select their answers and submit the exam.

4. Viewing Exam Results

- After submitting an exam, users can view their exam results.
- The exam results show the total score and the status of each question (correct, incorrect, or unanswered).

## License

This project is licensed under the Apache License. Feel free to use, modify, and distribute it as per the terms of the license.

## Credits

This Online Course Management System was developed as part of a Developing Applications with SQL, Databases, and Django course on Coursera. The project is based on the original work available at [https://github.com/ibm-developer-skills-network/final-cloud-app-with-database](https://github.com/ibm-developer-skills-network/final-cloud-app-with-database). The course and project were completed by benl2024.




