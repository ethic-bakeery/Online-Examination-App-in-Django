Online Examination Platform

Welcome to the Online Examination Platform, a comprehensive web application designed to manage exams, courses, questions, and student performance. This platform offers distinct functionalities for administrators, teachers, and students, enhancing the overall learning and assessment experience.
Features
Admin

    Account Creation: To create an admin account, use the following command: py manage.py createsuperuser.
    Dashboard: After logging in, admins can access an overview of the system, including the total number of students, teachers, courses, and questions.
    User Management: Admins have full control over user accounts. They can view, update, and delete teacher and student accounts. Admins can also approve teacher accounts.
    Course and Question Management: Admins can add, view, and delete courses/exams. They can add questions to specific courses, providing options, correct answers, and marks. Questions can also be viewed and deleted.
    Student Performance: Admins can view student marks for each attempt of every exam.
    Email Configuration: Admins can customize email settings in settings.py to facilitate communication with users.

Teacher

    Job Application: Teachers can apply for positions within the system, with approval required from the admin for login access.
    Dashboard: Upon login, teachers can see the total number of students, courses, and questions in the system.
    Course and Question Management: Teachers can add, view, and delete courses/exams. They can add questions to respective courses, including options, correct answers, and marks. Questions can also be viewed and deleted.

Student

    Account Creation: Students can create accounts without requiring admin approval.
    Dashboard: After login, students can view available courses/exams and the total number of questions in the system.
    Exam Participation: Students can attempt exams at any time, with no limits on the number of attempts. Exams consist of multiple-choice questions, each with 4 options and 1 correct answer.
    Performance Tracking: Students can view marks for each attempt of every exam.

How to Run the Project

    Python Installation: Ensure Python 3.7.6 is installed. During installation, select "Add to Path" for easier command execution.
    Install Dependencies: Open the terminal and execute the following command to install project dependencies:
    python -m pip install -r requirements.txt

Database Setup: Run the following commands to set up the database:

py manage.py makemigrations
py manage.py migrate

Run the Server: Start the development server using the following

    py manage.py runserver
    Access the Application: Open your web browser and enter the following URL:
    http://127.0.0.1:8000/

Drawbacks
Admins and teachers can add an unlimited number of questions to any course. However, when adding a course, admins must specify the total number of questions. This design choice may require further refinement based on specific project requirements.
