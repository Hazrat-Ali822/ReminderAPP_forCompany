# Reminder Application
This is a full-stack web application designed for hierarchical task management and reminders. The system includes a Django REST API back-end and a simple, responsive HTML/CSS/JavaScript front-end.

# Features
Role-Based Access Control: Differentiates user permissions based on roles: Super Admin, Admin, HR, and Manager.

Task Lifecycle: Manages tasks through a clear workflow, including pending, approved, and completed states.

Approval System: Tasks created by HR and Manager roles require approval from a designated Admin or Super Admin.

Dynamic Dashboard: Displays a personalized dashboard for each user role, complete with an interactive calendar and task lists.

Real-time Notifications: Admins and Super Admins are notified of pending tasks via a bell icon.

Getting Started
Follow these instructions to set up and run the project on your local machine.

Prerequisites
Python 3.10 or higher

Git (optional, but recommended)

# Installation

Create and activate a virtual environment:

python -m venv venv
# On Windows
.\venv\Scripts\activate

Install project dependencies:

pip install -r requirements.txt

Database Setup
# Run database migrations:

python manage.py makemigrations reminders
python manage.py migrate

Create a Super Admin account: This is the first user account and is created manually.

python manage.py createsuperuser

Follow the prompts to set a username and password.

Update Super Admin Role:

Run the Django development server: python manage.py runserver

Navigate to http://127.0.0.1:8000/admin/.

Log in with the Super Admin credentials.

Find the new user, edit their profile, and change the role from HR to Super Admin.

Running the Application
Start the Django back-end:

python manage.py runserver
