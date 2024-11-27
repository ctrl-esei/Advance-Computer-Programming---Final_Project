# Advance-Computer-Programming---Final_Project
This repository is for my final project in ACP - Advance Computer Programming

I.	PROJECT OVERVIEW: TIME4FITNESS MANAGEMENT SYSTEM

The Time4Fitness Management System is a comprehensive application designed to streamline fitness centre operations by combining gym membership management with exercise tracking. It caters to both gym members and administrators, providing a seamless experience for managing memberships, tracking activities, and overseeing equipment.

II.	Explanation of how python concepts, libraries, etc. were applied

1. Core Python Concepts
•	Functions:
o	Modular design is implemented using functions to encapsulate specific tasks, such as UserDashboard(), admin_UserLogin(), and databasejoin().
o	Promotes code reusability and clarity.
•	Error Handling:
o	Used try-except blocks to handle database connection errors, user input issues, and invalid operations gracefully.
o	Example: Handling invalid or missing input during registration to ensure data integrity.
•	Data Types:
o	Strings, integers, and enumerations (e.g., membership durations, equipment statuses).
o	Custom formatting for membership durations using logic and string manipulations.
•	Conditional Statements:
o	Validate user credentials and enforce constraints, such as checking for expired memberships before allowing actions.

2. Libraries and Their Applications

a. Tkinter and CustomTkinter
•	Purpose:
o	Build a modern and intuitive Graphical User Interface (GUI) for users and admins.
•	Applications:
o	Tkinter:
	Standard GUI elements like buttons, labels, entry fields, and treeviews.
	Example: Login, registration, and dashboard layouts.
o	CustomTkinter:
	Used for aesthetic enhancements (modern styling and themes).
	Example: Buttons with corner radius, color schemes, and responsive layouts.
o	Treeview:
	Display tabular data such as user details, attendance records, and equipment logs with scrollable views.
b. MySQL Connector
•	Purpose:
o	Interface with the MySQL database (FitnessDB) to perform CRUD operations.
•	Applications:
o	Query execution to fetch and update user, payment, attendance, and equipment data.
o	Example:
	Fetching available equipment: SELECT Equipment_ID, Equipment_Name, Status FROM Equipments.
	Logging exercises: INSERT INTO Exercise_Log.
•	Error Handling:
o	Ensures graceful degradation during connection failures or query execution errors.

c. Date and Time Libraries
•	Purpose:
o	Handle membership durations, attendance timestamps, and log dates.
•	Applications:
o	datetime.date.today():
	Retrieve the current date for operations like attendance marking.
o	datetime.timedelta:
	Calculate membership expiration dates.
o	datetime.datetime.now():
	Record precise timestamps for check-ins.

3. Advanced Concepts
•	Database Join Queries:
o	Combined data from multiple tables (e.g., Users, Memberships, Attendance) for comprehensive views.

4. Modular Code Design
•	Separate functions for distinct operations:
o	UI Windows: Functions like ExerciseLogWindow() and admin_UserLogin() create and manage specific interfaces.
o	Data Queries: Functions like equipmentNames() retrieve equipment data from the database.
o	Ensures maintainability and simplifies future expansions.

5. Additional Libraries
•	re (Regular Expressions):
o	Used for input validation, such as verifying email formats.
•	messagebox:
o	Display error, information, and warning dialogs to users.
o	Example: Informing users of expired memberships or payment submission status.

III.	Details of the Chosen SDG and its integration into the project

Goal 3: Good Health and Well-being the objective is to ensure healthy lives and promote well-being for all at all ages. This project supports Target 3.4 of SDG 3: "Reduce by one-third premature mortality from non-communicable diseases through prevention and treatment and promote mental health and well-being." The Time4Fitness Management System directly supports SDG 3 by promoting fitness, preventive health measures, and well-being for all members. Its efficient and inclusive design empowers gyms to better serve their communities, making healthy lifestyles more achievable and accessible.

IV.	Instructions for running the program


![Uploading image.png…]()

