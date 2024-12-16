Disaster Management System

Overview

The Disaster Management System is a comprehensive application designed to streamline disaster response and management processes. It enables users to report disasters in real time, coordinate response teams, and analyze historical data for improved preparedness and decision-making. Built using either Django or FastAPI, the system is adaptable to various operational needs.

Features

User Authentication: Secure login and account management.

Disaster Reporting: Submission of disaster details, including geolocation.

Resource Management: Allocation and tracking of response team resources.

Data Analytics: Insights and visualizations for trend analysis and strategic planning.

Tech Stack

Backend Frameworks: Django or FastAPI for robust API development.

Database: PostgreSQL for reliable data storage and retrieval.

Frontend: HTML, CSS, and JavaScript for user interfaces.

Getting Started

Prerequisites

Before setting up the project, ensure you have the following:

Python 3.8 or later

PostgreSQL database

Git for version control

Installation Steps

1. Clone the Repository

Retrieve the project files using:

git clone https://github.com/Ineza-Bernice/django.git
cd django

2. Set Up a Virtual Environment

Create an isolated Python environment to manage dependencies:

python3 -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

3. Install Dependencies

Use the requirements.txt file to install all necessary Python packages:

pip install -r requirements.txt

4. Configure Environment Variables

Create a .env file in the root directory with the following variables:

SECRET_KEY=your-secret-key
DEBUG=True
DATABASE_URL=postgres://user:password@localhost:5432/db_name

Replace your-secret-key, user, password, and db_name with your specific configuration.

5. Initialize the Database

Run the following commands to create and apply database migrations:

python manage.py makemigrations
python manage.py migrate

6. Start the Application Server

For Django:

python manage.py runserver

For FastAPI:

uvicorn app.main:app --reload

Accessing the Application

Web Interface

Django: Open http://127.0.0.1:8000 in your browser.

FastAPI: Navigate to http://127.0.0.1:8000/docs to explore the API using the interactive Swagger UI.

API Testing

Use tools like Postman or cURL to test endpoints. FastAPI’s integrated Swagger UI at /docs provides an interactive testing platform.

Project Structure

Here is an outline of the directory structure:
Django Directory Structure
DISASTER_MANAGEMENTS/
├── accounts/
├── disaster/
├── disaster_management/
├── myenv/
├── resources/
├── static/
├── templates/
├── db.sqlite3
├── manage.py
└── requirements.txt
FastAPI Directory Structure
DISASTER_MANAGEMENT/
├── __pycache__/
├── routers/
├── __init__.py
├── database.py
├── main.py
├── models.py
├── requirements.txt
├── schemas.py
└── utils.py
Contact Information

For support or inquiries, contact:

Name: Ineza Niyongira Bernice

Email: berniceneza1@gmail.com

