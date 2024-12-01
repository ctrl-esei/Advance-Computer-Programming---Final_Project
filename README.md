# Advance-Computer-Programming---Final_Project
This repository is for my final project in ACP - Advance Computer Programming
### Please note that i have coded in MacOS changes may apply when transfering the code to windows. Sorry for the inconvenience.

# Time4Fitness Management System

# I. Project Overview

The system called Time4Fitness purpose is to offer a comprehensive solution for the administration of gyms and fitness centers because it confronts management, members, and even data management and is issued in an effective way. Through automation of key activities like membership management, payment tracking, deleting members that wants their account to be deleted and even attendance recording, by these it takes the pressure off the administrators, and it promotes precision and reliability. In a matter of fact, this system offers its members the tools like exercise logs and attendance histories that they can keep track of their fitness development that helps to keep motivated.

This system allows for transparency and clarity by updating and making payment and membership records available to the members and administrators. Centralized databases enhance data management efficiency in features such as sales tracking, membership trend analysis, and reporting user statuses whether active or suspended. The framework enables participants in achieving their goals of good health and fitness while being characterized by building trust and transparency, hence commercial success, aligned to the organization’s mission. It creates opportunities for health clubs in terms of streamlining delivering excellent service to more constituents through eliminating redundancy and thus offering meaningful value. 

Therefore, the Time4Fitness system has been designed to enhance operational efficiency at the gym level so that memberships, transactions, exercise logs, and attendance records can be effectively managed. The feature allows registration of users, ensuring all aspects of membership are well covered, while administrators and members will be able to see records transparently. It tracks outstanding and fulfilled payments as well as exercise logs and attendance records, which are used to evaluate the progression of the user and engagement improvement. However, it requires the approval of an administrator instead of automatically during payment processing. Moreover, advanced functionalities, such as wearables or virtual training and complex data analytics, fall out of its scope. It is designed for the benefit of all those connected to it, from the gym administration, staff, trainers, to diverse members irrespective of their age. It is designed for access and usability, meaning that even a person without a lot of technical savvy or an elderly person can quickly use it without problems. The system accommodates a wide range of users with a simple and intuitive interface, thus making it fit for any person that would be managing or making use of the gym services.

The system will automate gym operations, including membership management, tracking payments, exercise logs, and attendance, reducing administrative workload by at least 50% six months after implementation. This shall enhance member participation through workout tracking and attendance log. This will thus ensure to enhance the retention rate of members up to 20% within the first year. The record of members along with payment records shall be made 100% accurate as data management will be centralized into an organized database. These include a 50% reduction in workload and a 20% increase in retention, that is, standard requirements found in studies on the digitalization of small and medium-sized businesses, such as fitness studios.

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

# III. SDG and its integration into the project

## SDG 3: Good Health and Well-Being
This goal is the main and the primary goal of the Time4Fitness Management system because it support its users and those who administer it in trying to encourage and help the people to regularly participate with an appreciation for and a preference for their health, all of which contributed towards the larger goal of healthier life while promoting well-being for everyone of all ages in whole wide world.

## SDG 9: Industry, Innovation, and Infrastructure
The system promotes innovation in the gym and fitness industry by developing and improving means of managing a gym via technology. The digital platform enhances operational effectiveness and saves manual work while providing improved member as well as administration experiences for the gym members.

## SDG 4: Quality Education
Time4Fitness Management System bring opportunities to the members and trainer also the administrators to learn about fitness, track their progress, and engage data-driven decision-making for health improvements. This helps us lifelong learning about fitness and well-being.

## SDG 12: Responsible Consumption and Production
By maintaining the proper document of fitness activities, membership details and the logs, the system makes management contributes practice more sustainable because I reduce the needs for paper documentation by that, it diminishes administrative inefficiencies, and it also promotes the wise use of resources of gym and fitness operations.


 # IV. Instruction for running the Program

1.	Download the zipped file.

2.	Unzip the files, the file contains both SQL and the code also the asset folder that contains the pictures of the code.

3.	Turn on Apache and MySQL and go to PHP my admin 

4.	In Phpmyadmin, create a database named FitnessDB and click on it.
 
5.	Once you clicked it, import the SQL that is included in the file. If you have encountered an error because the SQL is not zipped kindly compress the SQL.

6.	Now, after you have successfully imported the SQL into Phpmydamin you can now go to the Time4fitness.py.

7.	If you have encountered an error for the pictures, in the asset folder just copy the path and replace the path. It must’ve been because I have coded in different OS.

8.	If you want to enter the admin interface the admin’s password is admin as well as its username.

9.	Now, you can run the code.
