# Advance-Computer-Programming---Final_Project
This repository is for my final project in ACP - Advance Computer Programming

# Time4Fitness Management System

### I. Project Overview

The Time4Fitness Management System is a comprehensive application designed to streamline fitness center operations by combining gym membership management with exercise tracking. It caters to both gym members and administrators, providing a seamless experience for managing memberships, tracking activities, and overseeing equipment.

# II.	Explanation of how python concepts, libraries, etc. were applied

## 1. Core Python Concepts
* Functions:
    * Modular design is implemented using functions to encapsulate specific tasks, such as UserDashboard(), admin_UserLogin(), and databasejoin().
    * Promotes code reusability and clarity.
* Error Handling:
    * Used try-except blocks to handle database connection errors, user input issues, and invalid operations gracefully.
    * Example: Handling invalid or missing input during registration to ensure data integrity.
* Data Types:
    * Strings, integers, and enumerations (e.g., membership durations, equipment statuses).
    * Custom formatting for membership durations using logic and string manipulations.
* Conditional Statements:
    * Validate user credentials and enforce constraints, such as checking for expired memberships before allowing actions.

## 2. Libraries and Their Applications
### a. Tkinter and CustomTkinter
* Purpose:
    * Build a modern and intuitive Graphical User Interface (GUI) for users and admins.
* Applications:
    * Tkinter:
        * Standard GUI elements like buttons, labels, entry fields, and treeviews.
        * Example: Login, registration, and dashboard layouts.
    * CustomTkinter:
        * Used for aesthetic enhancements (modern styling and themes).
        * Example: Buttons with corner radius, color schemes, and responsive layouts.
    * Treeview:
        * Display tabular data such as user details, attendance records, and equipment logs with scrollable views.
          
### b. MySQL Connector
* Purpose:
    * Interface with the MySQL database (FitnessDB) to perform CRUD operations.
* Applications:
    * Query execution to fetch and update user, payment, attendance, and equipment data.
    * Example:
        * Fetching available equipment: SELECT Equipment_ID, Equipment_Name, Status FROM Equipments.
        * Logging exercises: INSERT INTO Exercise_Log.
* Error Handling:
    * Ensures graceful degradation during connection failures or query execution errors.
 
### c. Date and Time Libraries
* Purpose:
    * Handle membership durations, attendance timestamps, and log dates.
* Applications:
    * datetime.date.today():
        * Retrieve the current date for operations like attendance marking.
    * datetime.timedelta:
        * Calculate membership expiration dates.
    * datetime.datetime.now():
        * Record precise timestamps for check-ins.
 
### 3. Advanced Concepts
* Database Join Queries:
    * Combined data from multiple tables (e.g., Users, Memberships, Attendance) for comprehensive views.
 
### 4. Modular Code Design
* Separate functions for distinct operations:
    * UI Windows: Functions like ExerciseLogWindow() and admin_UserLogin() create and manage specific interfaces.
    * Data Queries: Functions like equipmentNames() retrieve equipment data from the database.
    * Ensures maintainability and simplifies future expansions.
 
### 5. Additional Libraries
* re (Regular Expressions):
    * Used for input validation, such as verifying email formats.
* messagebox:
    * Display error, information, and warning dialogs to users.
    * Example: Informing users of expired memberships or payment submission status.
 
