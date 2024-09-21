#1. Introduction
Overview: This Task Management System is a web application that allows users to create, manage, and track tasks efficiently. It provides a user-friendly interface for managing personal and departmental tasks.

Technologies Used
•	Backend: Django (Python)
•	Frontend: HTML, CSS, JavaScript
•	Database: PostgreSQL 
•	Version Control: Git

#2. Installation
Prerequisites
•	Python 3.12.0
•	pip (Python package installer)
•	PostgreSQL (optional, for production)
•	Git

Cloning the Repository
git clone https://github.com/diditeq/SE_Project.git
cd SE_Project.git

Setting Up a Virtual Environment
python -m venv 
On Windows use: `venv\Scripts\activate`

Installing Dependencies
pip install -r requirements.txt

#3 Configuration
Database Configuration
1.	Create a PostgreSQL database.
2.	Update settings.py with your database credentials.
Code:
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'your_db_name',
        'USER': 'your_db_user',
        'PASSWORD': 'your_db_password',
        'HOST': 'localhost',
        'PORT': '',
    }
}

Environment Variables
Create a .env file in the root directory and add your environment variables.
SECRET_KEY='your-secret-key'
DEBUG=True


#4. Running the Application
Migrations
python manage.py migrate
Starting the Development Server
python manage.py runserver
Visit http://127.0.0.1:8000 in your browser.

#5. Features
User Authentication
•	Users can register, log in, and log out.
Task Management
•	Creating Tasks: Users can create tasks with titles, descriptions, and due dates.
•	Updating Tasks: Edit task details as needed.
•	Deleting Tasks: Remove tasks that are no longer needed.
•	Task Prioritization: Assign priority levels to tasks.
•	Report: User can generate set task report 
•	Statistics: User can view Pending Task Statistics

Department Project Management
•	Department Categories are created and tasks are assigned to assignee in each department better organization.
User Roles and Permissions
•	Admin users can manage all tasks and users.
•	Regular users can view their own tasks, see deadlines for it and Generate Set Task Report.


#7. Testing
Running Tests
python manage.py test
Writing New Tests
•	Follow Django’s testing framework documentation for creating new tests.


#8. Deployment
Preparing for Production
•	Set DEBUG to False in settings.py.
•	Collect static files.
Code:
python manage.py collectstatic

Deployment on RENDER or Platform of your Choice
•	Follow the platform's deployment guides.


#9.Troubleshooting
Common Issues
•	Database connection errors.
•	Static files not loading.

##This documentation serves as a comprehensive guide for developers to understand, set up, and contribute to the project. Let me know if you need more specific details or sections!

