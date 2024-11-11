# Flask File Manager

A secure, multi-user file management system built with Flask that allows authenticated users to upload, download, and manage files through a web interface.


<img width="1437" alt="Screenshot 2024-11-11 at 3 36 04 PM" src="https://github.com/user-attachments/assets/3d891ed4-5a47-4486-b073-c12973f903c5">


<img width="1440" alt="Screenshot 2024-11-11 at 3 36 21 PM" src="https://github.com/user-attachments/assets/2e148819-5144-4812-938c-63a4075729b9">


<img width="1440" alt="Screenshot 2024-11-11 at 3 39 42 PM" src="https://github.com/user-attachments/assets/41131d96-9bb5-4c18-8906-5db045d4fcea">

## Features

- 🔐 Secure user authentication system
- 📤 File upload with extension validation
- 📥 File download functionality
- 🗑️ File deletion capabilities
- 🔒 Protected routes with login requirements
- 📁 Support for multiple file formats (txt, pdf, png, jpg, jpeg, gif, doc, docx, csv, xlsx, sql)
- 💾 SQLite database for user management
- 🎨 Clean and intuitive web interface

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/flask-file-manager.git
cd flask-file-manager
```

2. Create and activate a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

3. Install required packages:

```bash
pip install flask flask-login werkzeug flask-sqlalchemy
```

4. Configure the application:
   - Set your `UPLOAD_FOLDER` path in `app.py`
   - Change the `SECRET_KEY` to a secure value

5. Initialize the database:

```bash
python app.py
```

## Usage

1. Start the server:

```bash
python app.py

or flask run
```

2. Access the application at `http://localhost:5002`

3. Register a new account or login with existing credentials

4. Upload, download, and manage your files through the web interface

<<<<<<< HEAD
## NGROK

Use ngrok to create a http tunnel for a this project
=======
5. Use ngrok to create a http tunnel for this project
>>>>>>> 97d8d4e3382cde1b3440f838ac704fca6f01ef08

## Security Features

- Password hashing using Werkzeug security
- Secure filename handling
- Protected file operations
- Session management
- File extension validation

## Configuration

The following environment variables can be modified in `app.py`:

- `UPLOAD_FOLDER`: Directory where files will be stored
- `ALLOWED_EXTENSIONS`: Tuple of allowed file extensions
- `SECRET_KEY`: Application secret key for session management
- `SQLALCHEMY_DATABASE_URI`: Database connection string

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## Planned Updates

1. Feature to create folders
2. Check for file duplication
3. File upload records(uploader name, time, etc)
