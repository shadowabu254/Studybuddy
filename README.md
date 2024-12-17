StudyBud is a Django-powered web application that allows users to join study rooms, post messages, and interact with others. It demonstrates user authentication, CRUD operations, and dynamic data rendering using Django.
Table of Contents
        Project Overview
        Features
        Technologies Used
        Installation and Setup
        Usage
        Folder Structure
        Screenshots
        Credits
        Project Overview
        StudyBud is a platform for:
Functionalities:
        Joining study rooms where users can interact and learn together.
        Creating and managing rooms with specific topics.
        Sending messages within rooms to discuss subjects.
        Viewing and editing user profiles.

It demonstrates how to:

        Use Django for user authentication and dynamic content management.
        Perform CRUD operations.
        Structure and style a web application using Django templates.
        Features

User Authentication:
        Register, Login, and Logout functionality.

Study Rooms:
        Users can create, update, and delete rooms.
        View all study rooms on the home page.

Messaging:
        Users can send messages within rooms.

User Profiles:
        Update user profiles with bio, avatar, and other information.
        View other users' activities and rooms.

Dynamic Rendering:
        Displays real-time changes in rooms and messages.

Search Functionality:
        Search rooms by topic or name.

Technologies Used
        Backend:
                Django (Python)
        Frontend:
                HTML
                CSS
                JavaScript
        Database:
                SQLite (default) or any relational database
        Environment Management:
                Virtual Environment (venv)
        Other Libraries:
                Django Templates
                Bootstrap (for basic styling)

Installation and Setup
Follow these steps to set up the StudyBud project locally:

Prerequisites
Ensure you have:

        Python 3.x installed
        pip (Python package manager)
        A code editor (e.g., VSCode, PyCharm)
Steps:
Clone the repository:
        git clone https://github.com/shadowabu254/Studybuddy.git

Go To Project Directory Where You Cloned:
        cd Studybuddy

Set up a virtual environment:
        python3 -m venv venv
        source venv/bin/activate  # On Windows use `venv\Scripts\activate`

Install dependencies:
        pip install -r requirements.txt

Run migrations:
        python manage.py makemigrations
        python manage.py migrate

Create a superuser (admin account):
        python manage.py createsuperuser

Run the development server:
        python manage.py runserver

Access the app: Open your browser and visit:
        http://127.0.0.1:8000

Usage
Register or Log In:
        Go to the login page and create a new account or log in with your credentials.

Explore Rooms:
        View the available study rooms.
        Join a room to see messages and interact.

Create a Room:
        Use the "Create Room" option to start a new study discussion.

Send Messages:
        Post messages in a room and interact with others.

Update Profile:
        Edit your profile to include a name, bio, and avatar.
Project Folder Structure:
        studybud/
        │
        ├── base/                         # Core Django app
        │   ├── migrations/               # Database migrations
        │   ├── templates/                # HTML templates
        │   │   ├── base/                 # Main template files
        │   ├── static/                   # Static files (CSS, JS)
        │   ├── views.py                  # Django views
        │   ├── models.py                 # Database models
        │   ├── urls.py                   # App-level URLs
        │   └── forms.py                  # Forms for user input
        │
        ├── studybud/                     # Project-level folder
        │   ├── settings.py               # Project settings
        │   ├── urls.py                   # Project-level URLs
        │
        ├── db.sqlite3                    # SQLite database
        ├── manage.py                     # Django management script
        └── requirements.txt              # Project dependencies

Home Page:
        Displays all rooms and allows users to search.

Room Page:
        Shows room messages and allows message posting.

User Profile:
        Displays user-specific details and their activity.
