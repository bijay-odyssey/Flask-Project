# Flask Login with Google (OAuth 2.0)

This project demonstrates how to implement **Google OAuth 2.0 authentication** using Flask.  
It allows users to log in with their Google account and retrieves basic profile information after successful authentication.

The project is intended for learning how third-party authentication works in Flask applications.

---

## Features

- Google OAuth 2.0 login
- Secure session-based authentication
- Environment-based configuration for sensitive credentials
- Fetching user profile data from Google APIs
- Login and logout functionality

---

## Project Structure

```

loginwithgoogle/
│
├── app.py
├── myapp.env
└── README.md

````

---

## Tech Stack

- Python 3.x
- Flask
- requests-oauthlib
- python-dotenv
- OAuth 2.0 (Google)

---

## Getting Started

### 1. Install Dependencies

```bash
pip install flask requests-oauthlib python-dotenv
````

---

### 2. Configure Environment Variables

Create a `.env` file or update `myapp.env` with the following values:

```env
CLIENT_ID=your_google_client_id
CLIENT_SECRET=your_google_client_secret
REDIRECT_URI=http://localhost:5000/callback
```

Important: Do not commit real credentials to source control.

---

### 3. Run the Application

```bash
python app.py
```

Open your browser and visit:

```
http://localhost:5000
```

---

## OAuth Flow Overview

1. User clicks the login link
2. User is redirected to Google’s authentication page
3. Google redirects back to the application callback URL
4. Access token is stored in the session
5. User profile information is fetched from Google APIs

---

## Notes and Limitations

* HTTPS is disabled for local development using `OAUTHLIB_INSECURE_TRANSPORT`
* No persistent user storage is implemented
* This project is for learning purposes and not production-ready

---

## Learning Outcomes

* Understanding OAuth 2.0 authentication flow
* Integrating third-party login providers in Flask
* Managing access tokens and sessions
* Secure handling of environment variables
 
