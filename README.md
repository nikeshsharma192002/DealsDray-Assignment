# Employee Management System

This repository contains an Employee Management System built using React.js for the frontend and MongoDB for the backend. The application includes features for managing employee data and user authentication.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup Instructions](#setup-instructions)
- [Database Schema](#database-schema)
- [Validations](#validations)
- [Login Management](#login-management)
- [License](#license)

## Features

- User authentication (login and logout)
- Manage employee details (CRUD operations)
- Display user information on the dashboard
- Server-side and client-side form validations

## Technologies Used

- **Frontend**: React.js, JavaScript, HTML, CSS
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Libraries**: jQuery, Bootstrap (optional for styling)

## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/nikeshsharma192002/DealsDray-Assignment/
   cd DealsDray-Assignment

2. **Install dependencies**:

   For the backend, navigate to the server directory and run:
   ```bash

    cd backend
    npm install
  For the frontend, navigate to the client directory and run:
  ``bash
    
    cd frontend
    npm install
  Configure the MongoDB database:

  Make sure you have MongoDB installed and running on your machine.
  Create the necessary tables in the database by running the MongoDB scripts provided in the Database Schema section.
  Run the application:

  Start the backend server:
  ``bash
    cd backend
    npm start
   Start the frontend development server:
``bash

    cd frontend
    npm start
  Access the application:

Open your browser and navigate to http://localhost:3000 to access the application.
Database Schema
t_login
Field	Description
f_sno	Serial number (Primary Key)
f_userName	Username for login
f_Pwd	Password for login
t_Employee
Field	Description
f_Id	Employee ID (Primary Key)
f_Image	Employee profile image
f_Name	Employee name
f_Email	Employee email address
f_Mobile	Employee mobile number
f_Designation	Employee designation
f_gender	Employee gender
f_Course	Course assigned to the employee
f_Createdate	Employee record creation date
Validations
The application includes both server-side and client-side validations to ensure data integrity.

Client-Side Validation
Implemented using JavaScript and jQuery.
Validates form inputs on the client side before submission.
Checks for empty fields, email format, and other necessary validations.
Server-Side Validation
Implemented in the backend using Express.js middleware.
Validates form inputs on the server side after submission.
Ensures secure and consistent data handling.
Login Management
The login functionality validates user credentials against the t_login table in the database.
On successful login, the user is redirected to the dashboard.
If login credentials are invalid, an alert is shown with the message "Invalid login details."
The username is displayed on the dashboard using local storage or cookies.
React.js and MongoDB are used to manage the user session and state.

## License
This project is licensed under the MIT License - see the LICENSE file for details.



