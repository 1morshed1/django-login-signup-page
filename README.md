# Django-Login-Signup-Page

A simple and secure Django project demonstrating user authentication with login and signup functionalities. This project serves as a foundational boilerplate for building web applications requiring user management.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Application](#running-the-application)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **User Registration**: Secure signup with username, email, and password
- **User Login**: Authenticate users with their credentials
- **User Logout**: Securely log users out of their sessions
- **Password Hashing**: Uses Django's built-in robust password hashing for security
- **Session Management**: Handles user sessions securely
- **Basic UI**: Simple and clean user interface for login and signup forms
- **Admin Panel Integration**: Users created via the application are accessible and manageable through Django's powerful admin interface

## Technologies Used

- **Backend**: Python 3.x, Django 5.x
- **Database**: SQLite (default, easily configurable for PostgreSQL, MySQL, etc.)
- **Frontend**: HTML, CSS (minimal styling)

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.x (download from [python.org](https://python.org))
- pip (Python package installer, usually comes with Python)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/1morshed1/django-login-signup-page.git
   cd django-login-signup-page
   ```

2. **Create a virtual environment (recommended):**
   ```bash
   python -m venv venv
   ```

3. **Activate the virtual environment:**
   
   **On Windows:**
   ```bash
   .\venv\Scripts\activate
   ```
   
   **On macOS/Linux:**
   ```bash
   source venv/bin/activate
   ```

4. **Install the required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

5. **Apply database migrations:**
   ```bash
   python manage.py migrate
   ```

6. **Create a superuser (optional, for accessing the Django admin panel):**
   ```bash
   python manage.py createsuperuser
   ```
   Follow the prompts to create your superuser account.

### Running the Application

1. **Start the Django development server:**
   ```bash
   python manage.py runserver
   ```

2. **Access the application:**
   Open your web browser and navigate to `http://127.0.0.1:8000/`

## Usage

- **Homepage**: `http://127.0.0.1:8000/` (or your configured root URL)
- **Signup**: Navigate to `/signup/` (e.g., `http://127.0.0.1:8000/signup/`) to create a new user account
- **Login**: Navigate to `/login/` (e.g., `http://127.0.0.1:8000/login/`) to log in with an existing account
- **Logout**: Once logged in, you can log out by navigating to `/logout/` (e.g., `http://127.0.0.1:8000/logout/`)
- **Admin Panel**: If you created a superuser, you can access the admin panel at `/admin/` (e.g., `http://127.0.0.1:8000/admin/`)

## Project Structure

```
signupProject/
├── manage.py
├── signupProject/                 # Main project settings
│   ├── __init__.py
│   ├── settings.py               # Project configuration
│   ├── urls.py                   # Main URL dispatcher
│   └── wsgi.py
├── users/                        # User app for authentication
│   ├── migrations/
│   ├── templates/
│   │   └── users/
│   │       ├── login.html
│   │       ├── signup.html
│   │       └── dashboard.html    # For logged-in users
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py                  # Custom forms (e.g., UserCreationForm)
│   ├── models.py
│   ├── urls.py                   # App-specific URL dispatcher
│   └── views.py                  # Logic for login, signup, etc.
├── requirements.txt              # Project dependencies
└── README.md
```

## Contributing

Contributions are welcome! If you have suggestions for improvements, please feel free to:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some feature'`)
5. Push to the branch (`git push origin feature/YourFeature`)
6. Open a Pull Request


## Contact

**Your Name** - morshedfahim87@gmail.com
**Project Link**: https://github.com/1morshed1/django-login-signup-page

---

⭐ If you found this project helpful, please give it a star on GitHub!