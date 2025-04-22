# Task Manager

A simple web-based task management application built with Flask and SQLAlchemy that allows users to create, update, and delete tasks.

## Features

- Create new tasks
- View all tasks in a clean interface
- Update existing tasks
- Delete tasks when completed
- Tasks are stored with their creation date


## Technologies Used

- **Flask** - Web framework
- **SQLAlchemy** - ORM for database operations
- **SQLite** - Database for storing tasks
- **HTML/CSS** - Frontend interface

## Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/YasithGunawardhana/task-manager.git
cd task-manager
```

2. Create and activate a virtual environment (recommended):
```bash
python -m venv venv
```

On Windows:
```bash
venv\Scripts\activate
```

On macOS/Linux:
```bash
source venv/bin/activate
```

3. Install the required dependencies:
```bash
pip install -r requirements.txt
```

4. Initialize the database:
```bash
python
>>> from app import app, db
>>> with app.app_context():
>>>     db.create_all()
>>> exit()
```

## Usage

1. Start the application:
```bash
python app.py
```

2. Open your web browser and navigate to:
```
http://127.0.0.1:5000/
```

3. Use the interface to:
   - Add new tasks using the form at the bottom
   - View your tasks in the table
   - Update tasks by clicking the "Update" link
   - Delete tasks by clicking the "Delete" link

## Project Structure

```
task-manager/
├── app.py                  # Main application file
├── requirements.txt        # Python dependencies
├── static/                 # Static files
│   └── css/
│       └── main.css        # Styling for the application
├── templates/              # HTML templates
│   ├── base.html           # Base template
│   ├── index.html          # Main page template
│   └── update.html         # Update task template
└── README.md               # This file
```

## Future Improvements

- Add user authentication
- Implement task categories/priorities
- Add due dates for tasks
- Improve mobile responsiveness
- Add search functionality
- Implement task completion status

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

Yasith Gunawardhana

---

Feel free to contribute to this project by submitting pull requests or reporting issues!