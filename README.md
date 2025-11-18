# LIBRARY MANAGEMENT SYSTEM 
# Description / Overview 
This Laravel-based CRUD MVC web application was created to efficiently manage library resources, including books, members, and borrowing/returning transactions. It was developed as part of the Midterm Examination for the IT course in SYSTEM INTEGRATION.
# Objectives
The Library Management System enables administrators and librarians to easily add, view, edit, and remove records while also tracking book borrowing and return activities. It is built using the Model-View-Controller (MVC) design pattern to ensure a well-structured and maintainable system.
# Features / Functionality 
•	Add, edit, delete, and view detailed book information
•	Manage member records, including students, teachers, and other users
•	Search and filter books quickly for easier access
•	Responsive and user-friendly interface built with Blade templates
•	Supports database migration and seeding for smooth setup
   **Model (M)**
    -Book.php
    -Borrowing.php
    -Students.php
    -User.php
 **View (V)**
    -resources/views/books/index.blade.php
    -resources/views/books/create.blade.php
    --resources/views/books/show.blade.php
   **Controller (C)**
    -BookController.php
    -BorrowingController.php
    -Controller.php
    -StudentController.php
# CRUD Operations
Operation	HTTP Method	Description	Example Route
Create	POST	Adds a new record to the collection.	/books
Read	Get	Retrieves and displays a list of records.	/books
Update	PUT/PATCH	Modifies the details of an existing record.	/books {id}
Delete 	DELETE	Removes a record from the collection.	/books {id}
