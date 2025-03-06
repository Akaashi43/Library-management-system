
# Library Management System

## Project Overview
The **Library Management System** is a web-based application built using the **Django framework**. It allows library administrators to manage books, users, and transactions efficiently. The system provides an interactive platform for managing book records, issuing books, returning books, and keeping track of users' borrowing history.

## Features
- **User Authentication**: Secure login and registration system for users.
- **Book Management**: Add, update, delete, and search books.
- **User Management**: Register new users and manage existing users.
- **Book Issue & Return System**: Borrow and return books with due date tracking.
- **Fine Calculation**: Automatically calculates late fees for overdue books.
- **Dashboard**: Overview of issued books, returned books, and available stock.
- **Admin Panel**: Manage users, books, and transactions via Django's built-in admin interface.

## Technologies Used
- **Backend**: Django (Python)
- **Frontend**: HTML, CSS, Bootstrap
- **Database**: SQLite (can be configured for PostgreSQL or MySQL)
- **Authentication**: Django’s built-in authentication system

## Installation Guide

### Prerequisites
Ensure you have the following installed on your system:
- Python (3.x)
- Django (latest version)
- SQLite (default with Django) or PostgreSQL/MySQL (if configured)

### Setup Instructions
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-repository/library-management.git
   cd library-management
   ```

2. **Create a virtual environment (Optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # For Linux/Mac
   venv\Scripts\activate  # For Windows
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply migrations:**
   ```bash
   python manage.py migrate
   ```

5. **Create a superuser for admin access:**
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the server:**
   ```bash
   python manage.py runserver
   ```

7. **Access the application:**
   Open your browser and go to `http://127.0.0.1:8000/`

## Project Structure
```
Library-Management/
│── library_management/   # Main Django project folder
│   ├── settings.py       # Django settings
│   ├── urls.py           # URL routing
│   ├── wsgi.py           # WSGI configuration
│── books/                # App to manage books
│   ├── models.py         # Database models
│   ├── views.py          # Business logic
│   ├── urls.py           # App URL patterns
│   ├── templates/        # HTML templates
│── users/                # User authentication and management
│── static/               # CSS, JavaScript, Images
│── db.sqlite3            # SQLite database (default)
│── manage.py             # Django command-line tool
```

## Future Enhancements
- Add book reservation feature.
- Implement barcode scanning for book entries.
- Improve UI/UX for a better user experience.
- Integrate email notifications for due dates.





