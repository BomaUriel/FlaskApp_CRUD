# Task Smash 2.0 - Flask CRUD Application

A simple Flask-based task management application with Create, Read, Update, and Delete (CRUD) functionality. Users can add, view, edit, and delete tasks with persistent storage using SQLite.

## Features

- Add new tasks
- View all tasks with creation date
- Edit existing tasks
- Delete tasks
- Persistent database storage with SQLite
- Responsive design with custom styling

## Tech Stack

- **Backend:** Flask 3.1.3
- **Database:** SQLite with SQLAlchemy ORM
- **Frontend:** Jinja2 templates with HTML/CSS
- **Styling:** SCSS compiled to CSS

## Prerequisites

- Python 3.8 or higher
- pip, the Python package manager

## Setup Instructions

### 1. Clone the Repository

```bash
git clone [repository-url](https://github.com/BomaUriel/FlaskApp_CRUD.git)
cd FlaskApp_CRUD
```

### 2. Create a Virtual Environment

```bash
python -m venv .venv
```

### 3. Activate the Virtual Environment

On Windows with Git Bash/MINGW64:

```bash
source .venv/Scripts/activate
```

On Windows with PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

On macOS/Linux:

```bash
source .venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the Application

```bash
python app.py
```

The application will start at:

```text
http://127.0.0.1:5000/
```

Open that URL in your browser. Debug mode is enabled, so the server reloads automatically when code changes. Press `CTRL+C` in the terminal to stop the server.

## Project Structure

```text
FlaskApp_CRUD/
|-- app.py                 # Main Flask application
|-- requirements.txt       # Python dependencies
|-- README.md              # Project documentation
|-- .venv/                 # Virtual environment, not committed to git
|-- instance/
|   `-- database.db        # SQLite database, auto-created
|-- static/
|   |-- styles.css         # Compiled CSS
|   `-- styles.scss        # SCSS source
`-- templates/
    |-- base.html          # Base template
    |-- index.html         # Task list page
    `-- edit.html          # Edit task page
```

## Database

- **Type:** SQLite
- **Location:** `instance/database.db`
- **Auto-created:** Yes, on first run
- **Table:** `MyTask`

`MyTask` columns:

- `id` - Integer, primary key
- `content` - String, max 100 characters
- `complete` - Integer, default 0
- `created` - DateTime

## Dependencies

See `requirements.txt` for the complete list. Main packages include:

- Flask
- Flask-SQLAlchemy
- Jinja2

## Future Enhancements

- User authentication
- Task categories or tags
- Due dates and reminders
- Task priority levels
- Search functionality
- Production deployment

## License

This project is open source and available under the MIT License.

## Author

Created by BOMAU
