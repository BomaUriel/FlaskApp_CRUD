# Task Smash 2.0 - Flask CRUD Application

A simple Flask-based task management application with Create, Read, Update, and Delete (CRUD) functionality. Users can add, view, edit, and delete tasks with persistent storage using SQLite.

## Features

- ✅ Add new tasks
- ✅ View all tasks with creation date
- ✅ Edit existing tasks
- ✅ Delete tasks
- ✅ Persistent database storage with SQLite
- ✅ Responsive design with custom styling

## Tech Stack

- **Backend:** Flask 3.1.3
- **Database:** SQLite with SQLAlchemy ORM
- **Frontend:** Jinja2 templates with HTML/CSS
- **Styling:** SCSS (compiled to CSS)

## Prerequisites

- Python 3.8 or higher
- pip (Python package manager)

## Setup Instructions

### 1. Clone the Repository
```bash
git clone <repository-url>
cd FlaskApp_CRUD

2. Create a Virtual Environment
python -m venv .venv

3. Activate Virtual Environment
On Windows (Git Bash/MINGW64):
source .venv/Scripts/activate

On macOS/Linux:
source .venv/bin/activate


4. Install Dependencies
pip install -r requirements.txt
Running the Application

python app.py
The application will start on http://127.0.0.1:5000/

Open your browser and navigate to the URL
Debug mode is enabled (auto-reloads on code changes)
Press CTRL+C to stop the server


Project Structure

FlaskApp_CRUD/
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── README.md             # This file
├── database.db           # SQLite database (auto-created)
├── instance/             # Instance folder for app data
├── static/               # Static files
│   ├── styles.css       # Compiled CSS
│   └── styles.scss      # SCSS source
├── templates/            # HTML templates
│   ├── base.html        # Base template
│   ├── index.html       # Task list page
│   └── edit.html        # Edit task page
└── env/                 # Virtual environment (not committed to git)


Database
Type: SQLite
Location: database.db
Auto-created: Yes (on first run)
Table: MyTask with columns:
id (Integer, Primary Key)
content (String, max 100 chars)
complete (Integer, default 0)
created (DateTime)


Dependencies
See requirements.txt for complete list. Main packages:

Flask
Flask-SQLAlchemy
Jinja2


Future Enhancements
 User authentication
 Task categories/tags
 Due dates and reminders
 Task priority levels
 Search functionality
 Deployment to production

 
License
This project is open source and available under the MIT License.

Author
Created by BOMAU