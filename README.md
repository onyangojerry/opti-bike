# opti-bike
An attempt to optimize bike usage on campus

This repository contains the OptiBike project, a Django-based web application.

Project Overview

The OptiBike project is designed using the Django web framework. It follows the Model-View-Controller (MVC) pattern and is intended to be deployed using ASGI and WSGI for asynchronous and synchronous communication, respectively.

Key Features:
ASGI configuration for handling asynchronous tasks.
WSGI configuration for handling synchronous tasks.
Basic settings for database, middleware, and templates using the default SQLite database.
Password validators to ensure secure authentication.
URLs mapped to Django admin and other app views.
Requirements

The following dependencies are needed for the project to run:

Django >= 3.2, < 4.0
djangorestframework (if using Django REST Framework for building APIs)
requests (for making HTTP requests, e.g., Google Maps API)
googlemaps (for Google Maps API integration)
You can install the dependencies using pip:

bash
Copy code
pip install -r requirements.txt
Project Structure

ASGI Configuration: Located in asgi.py, used for handling asynchronous server communication.
WSGI Configuration: Located in wsgi.py, used for handling synchronous server communication.
Settings: Defined in settings.py, this file contains project-wide configurations like installed apps, middleware, and database settings.
URLs: Defined in urls.py, which maps the URLs to the corresponding views.
Database: Uses SQLite by default. You can modify the DATABASES setting in settings.py for a different database backend.
Running the Project

To run the project locally, follow these steps:

Clone the repository:
bash
Copy code
git clone https://github.com/yourusername/optibike.git
Navigate to the project directory:
bash
Copy code
cd optibike
Install the dependencies:
bash
Copy code
pip install -r requirements.txt
Run the development server:
bash
Copy code
python manage.py runserver
The server will start, and you can access the project by visiting http://localhost:8000.

Security Notes

Keep your SECRET_KEY secret in production.
Set DEBUG = False in production environments.
Add allowed hosts in the ALLOWED_HOSTS setting to restrict access.
Deployment

For deploying the project, you can use platforms like Heroku, AWS, or any other cloud platform. Make sure to configure environment variables and update the settings accordingly.

For more information, see the Django deployment checklist.

This project was built using Django 4.2.3. For further details about Django, refer to the official documentation.
