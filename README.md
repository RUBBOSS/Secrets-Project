# Secrets Project

# Overview

This project is a web application that allows users to share their secrets anonymously. Users can register, log in, and submit their secrets securely. The app also supports Google authentication.

# Features

User Authentication: Users can register and log in with their email and password. Google authentication is also supported.
Secret Sharing: Once logged in, users can submit their secrets anonymously.
Responsive Design: The application is built to be responsive and user-friendly on all devices.
Getting Started
Prerequisites
Before you begin, ensure you have the following installed on your system:

Node.js (v14.x or higher)
PostgreSQL (v12 or higher)

# Installation

1.  Clone the repository:

    git clone https://github.com/RUBBOSS/secrets-project.git
    cd secrets-project

2.  Install dependencies:
    npm install

3.  Configure environment variables:
    Create a .env file in the root of your project and add the following:

    GOOGLE_CLIENT_ID=your-google-client-id
    GOOGLE_CLIENT_SECRET=your-google-client-secret
    SESSION_SECRET=your-session-secret
    PG_USER=your-postgres-username
    PG_HOST=localhost
    PG_DATABASE=secrets
    PG_PASSWORD=your-postgres-password
    PG_PORT=5432

4. Set up the PostgreSQL database:

    Create a database named secrets.
    Ensure the credentials in the .env file match your PostgreSQL setup.

5. Run the application:

    npm start

The server will start on http://localhost:3000.

# Usage

    Register: Go to http://localhost:3000/register to create a new account.
    Log In: Use your credentials or Google account to log in.
    Submit a Secret: Once logged in, go to Submit Secret to share your secret.

# Project Structure

    public/: Contains static assets like CSS, images, etc.
    views/: Contains EJS templates for rendering HTML.
    index.js: The main server file, handling routes, authentication, and database interactions.

# Dependencies

`express`: Web framework for Node.js
`ejs`: Template engine for rendering HTML
`body-parser`: Middleware for parsing request bodies
`bcrypt`: Library for hashing passwords
`passport`: Authentication middleware
`passport`-local: Local strategy for authentication using email and password
`passport`-google-oauth2: Google authentication strategy
`express-session`: Middleware for managing sessions
`pg`: PostgreSQL client for Node.js
`dotenv`: Loads environment variables from .env file