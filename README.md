# User Registration System

A full-stack web application that provides CRUD functionality for user registration.

## Features

- View a list of registered users
- Add new users with name, email, date of birth, and optional fields
- Update existing user information
- Delete users from the database
- Form validation and error handling
- Responsive UI design

## Technology Stack

- **Backend**: Python with Flask, SQLAlchemy
- **Frontend**: HTML, CSS, JavaScript (Vanilla)
- **Database**: SQLite (can be easily changed to MySQL or PostgreSQL)

## Project Structure

```
registration-system/
├── backend/
│   ├── app.py
│   └── instance/
│       └── registration.db
├── frontend/
│   ├── index.html
│   ├── css/
│   │   └── styles.css
│   └── js/
│       └── script.js
└── README.md
```

## Setup Instructions

### Backend Setup

1. Navigate to the backend directory:
   ```
   cd backend
   ```

2. Create a virtual environment:
   ```
   python -m venv venv
   ```

3. Activate the virtual environment:
   - Windows:
     ```
     venv\Scripts\activate
     ```
   - macOS/Linux:
     ```
     source venv/bin/activate
     ```

4. Install dependencies:
   ```
   pip install flask flask-sqlalchemy flask-cors
   ```

5. Run the application:
   ```
   python app.py
   ```

   The backend server will start running at http://localhost:5000

### Frontend Setup

1. Navigate to the frontend directory:
   ```
   cd frontend
   ```

2. Open the `index.html` file in your browser:
   - You can use a local server like Python's built-in HTTP server:
     ```
     python -m http.server
     ```
     Then visit http://localhost:8000

   - Or you can use extensions like Live Server in Visual Studio Code

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/users | Get all users |
| GET | /api/users/:id | Get user by ID |
| POST | /api/users | Create a new user |
| PUT | /api/users/:id | Update a user |
| DELETE | /api/users/:id | Delete a user |

## Future Improvements

- Add authentication and user roles
- Implement pagination for large datasets
- Add search and filtering functionality
- Create unit tests for backend and frontend
- Deploy to a production environment
