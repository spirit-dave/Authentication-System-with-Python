# REST API

A robust Authentication System built using Python's Flask framework. This API handles user registration, login, token-based authentication, and secure password management. It is designed to integrate seamlessly with any application that requires user authentication.

## Features

User Registration: Allow users to sign up with unique credentials.

User Login: Authenticate registered users and provide access tokens.

Token-Based Authentication: Secure endpoints with JWT (JSON Web Token).

Password Security: Passwords are hashed and stored securely using bcrypt.

User Management: Retrieve and manage user profiles.

## Technologies Used

Python: Core programming language.

Flask: Framework for creating REST APIs.

Flask-JWT-Extended: Library for implementing JWT authentication.

bcrypt: Used for password hashing and verification.

SQLite: Lightweight database for data storage.

## Project Structure

├── app.py             # Main application file

├── models.py          # Contains database models

├── routes.py          # Defines API routes

├── auth.db            # SQLite database (auto-created on first run)

├── config.py          # Configuration settings

└── requirements.txt   # List of dependencies

## Setup and Installation

1. Clone the Repository
Clone the repository using the command:

git clone https://github.com/yourusername/authentication-system.git
cd authentication-system

2. Create a Virtual Environment
Create and activate a virtual environment:


3. Install Dependencies

Install the required dependencies from the requirements.txt file:

4. Run the Application

Start the Flask server

5. Test the API
Use Postman or another tool to interact with the API

## Setup and Installation

1. Clone the Repository

Clone the repository using your preferred Git client.

2. Create a Virtual Environment

Set up a virtual environment to isolate dependencies.

3. Install Dependencies

Install required dependencies from the requirements.txt file.

4. Run the Application

Start the Flask server to host the API locally.

5. Test the API

Use Postman or any API testing tool to interact with the endpoints.

## API Endpoints

1. Register User

Endpoint: POST /register

Description: Register a new user with unique credentials.

2. Login User

Endpoint: POST /login

Description: Authenticate users and generate a JWT for secure access.

3. Get User Profile

Endpoint: GET /profile

Description: Retrieve the authenticated user’s profile.

Headers: Requires a valid Authorization: Bearer <token> header.

4. Logout User

Endpoint: POST /logout

Description: Revoke the user’s access token.

5. Update User Details

Endpoint: PUT /update-profile

Description: Modify user account details.

Headers: Requires a valid Authorization: Bearer <token> header.

## Database

The system uses SQLite to store user credentials and profile information. Passwords are hashed using bcrypt for security.

## User Model

Field	Type	Description
id	Integer	Primary key
username	String	Unique username for the user
password	String	Hashed password
Future Enhancements
Add role-based access control (e.g., admin vs. standard user).
Integrate multi-factor authentication (MFA) for enhanced security.
Enable email verification for new users.
Support OAuth2 or third-party login (e.g., Google, Facebook).

Contact
For any questions or feedback, contact adeyemi.b.david@gmail.com
