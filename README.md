# Calculator Web Application

## Overview

This is a simple Java EE web application built using Servlets and JSP, providing the following features:

- User registration and login
- A calculator page with history tracking
- Display of registered users
- Access control via a servlet filter
- Custom 404 error page
- Styling using Bootstrap and custom CSS

## Technologies Used

-	Java 11
- Servlet API
-	JSP
-	HTML5 / CSS3
-	Bootstrap 5
-	Apache Tomcat 10

## Setup and Running

1. Import the project into your favorite IDE (Eclipse, IntelliJ IDEA).
2. Make sure you have a servlet container like Apache Tomcat (version 10 or higher) installed.
3. Build and deploy the WAR to your servlet container.
4. Access the application at `http://localhost:8080/CalculatorWebApp/jsp/register.jsp` to register a new user.
5. After login, you will be able to access the calculator page and the list of registered users.

## Features

### Registration and Login

- Users can register with a username and password.
- Login form validates user credentials.

### Calculator Page

- Users can perform calculations.
- The calculation history is saved and can be cleared.

### User List

- Displays all registered usernames.
- Protected by `AuthFilter` — only logged-in users can access.

### Access Control

- `AuthFilter` restricts access to sensitive pages and servlets.
- Redirects unauthorized users to the login page.

### Error Handling

- Custom 404 error page (`error404.jsp`) for invalid URLs.

## How to Extend

- Implement password hashing in DAO for security.
- Add email verification on registration.
- Improve UI with custom styles in `style.css`.
- Add user roles and role-based authorization.
- Persist data in a database instead of in-memory or simple storage.
