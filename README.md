File Sharing Web Application
This repository contains a simple and secure file-sharing web application built with Flask. The app allows users to upload, download, and manage files, with user authentication and file security.

Features
User Authentication: Secure login system using Flask-Login and hashed passwords.
File Upload & Download: Users can upload various file types (e.g., txt, pdf, png, jpg, etc.) to a designated folder on the server.
Database Management: Stores user credentials in a SQLite database using SQLAlchemy.
Security: File uploads are sanitized, and user sessions are managed with secure authentication.
Setup and Installation
Clone the repository and navigate to the project folder:

bash
Copy code
git clone <repository-url>
cd file-sharing-app
Install the required packages:

bash
Copy code
pip install -r requirements.txt
Configure the environment variables:

Update the UPLOAD_FOLDER path and SECRET_KEY in the app.py file as needed.
Initialize the database:

bash
Copy code
flask db init
flask db migrate
flask db upgrade
Start the application:

bash
Copy code
flask run
Usage
Upload Files: Upload files of allowed types to share securely.
Download Files: Access files securely via the web interface.
Authentication: Only registered users can upload and download files.
