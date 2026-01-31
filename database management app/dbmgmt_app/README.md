# Database Management Flask Application

This project is a **Flask-based database management application** that allows an administrator to dynamically create and modify database tables through a web interface.

It is designed as a learning project to understand database introspection, schema manipulation, and admin-restricted access in Flask.

---

## Features

- Admin-only authentication
- Login and logout using Flask-Login
- Create new database tables dynamically
- View existing tables
- Add new columns to tables
- Delete existing columns
- Define foreign key relationships
- SQLite database integration
- SQLAlchemy metadata reflection

---

## Project Structure

```

dbmgmt_app/
│
├── static/
│   └── style.css
│
├── templates/
│   ├── base.html
│   ├── login.html
│   ├── dashboard.html
│   └── table_edit.html
│
├── app.py
├── requirements.txt
└── database.db

````

---

## Tech Stack

- Python 3.x
- Flask
- Flask-SQLAlchemy
- Flask-Login
- SQLAlchemy
- SQLite
- Jinja2 Templates
- HTML and CSS

---

## Getting Started

### 1. Install Dependencies

```bash
pip install -r requirements.txt
````

---

### 2. Run the Application

```bash
python app.py
```

---

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

## Application Overview

* Only admin users can access the dashboard
* Tables are created dynamically at runtime
* Database schema is reflected using SQLAlchemy metadata
* Table structure can be modified without restarting the application

---

## Notes and Limitations

* This project is intended for educational purposes only
* Uses raw SQL for altering tables
* SQLite has limited support for dropping columns
* No role management beyond a single admin user
* Not suitable for production environments

---

## Learning Outcomes

* Flask authentication and authorization
* Dynamic database schema manipulation
* SQLAlchemy metadata reflection
* Combining ORM and raw SQL
* Admin-only application design
 
