# Basic CRUD Flask Application

This project is a **Flask-based CRUD application** that demonstrates user authentication, role-based access control, and basic database operations using SQLite and SQLAlchemy.

It is designed as a practice project to understand Flask fundamentals, authentication flows, and database interactions.

---

## Features

- User registration with email validation
- Secure password hashing using Werkzeug
- Login and logout with Flask-Login
- Role-based access control (Admin and User)
- Admin dashboard to manage users
- Update user details and reset passwords
- Delete users (admin-restricted)
- Flash messaging for user feedback
- SQLite database integration

---

## Project Structure

```

basic-crud/flask_app
│
├── static/
│   └── style.css
│
├── templates/
│   ├── base.html
│   ├── login.html
│   ├── register.html
│   ├── user_dashboard.html
│   └── admin_dashboard.html
│
├── app.py
├── requirements.txt
└── users.db

````

---

## Tech Stack

- Python 3.x
- Flask
- Flask-SQLAlchemy
- Flask-Login
- Werkzeug
- email-validator
- SQLite
- HTML and CSS

---

## Getting Started

### 1. Install Dependencies

```bash
pip install -r requirements.txt
````

### 2. Run the Application

```bash
python app.py
```

### 3. Open in Browser

```
http://127.0.0.1:5000
```

---

## Default Admin Credentials

On first run, an admin user is automatically created:

```
Username: admin
Password: admin123
```

---

## Application Flow

1. Users can register with a valid email address
2. Users log in using their credentials
3. Admin users are redirected to the admin dashboard
4. Non-admin users are redirected to the user dashboard
5. Admin users can manage all registered users

---

## Notes and Limitations

* This project is intended for learning purposes only
* Error handling and security are minimal
* API keys and secrets should not be hardcoded
* Not suitable for production use

---

## Learning Outcomes

* Flask routing and templates
* User authentication and session handling
* Role-based authorization
* ORM usage with SQLAlchemy
* Basic CRUD operations

 
