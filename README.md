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
## CRUD Operations
| Operation | HTTP Method | Description | Example Route |
| :--- | :---: | :--- | :--- |
| Create | POST | Adds a new record to the collection. | `/books` |
| Read | GET | Retrieves and displays a list of records. | `/books` |
| Update | PUT/PATCH | Modifies the details of an existing record. | `/books/{id}` |
| Delete | DELETE | Removes a record from the collection. | `/books/{id}` |

## 🚀 Installation Instructions

1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/](https://github.com/)<your-username>/SALTIVAN-LIB-TPS.git
    cd SALTIVAN-LIB-TPS
    ```

2.  **Install Dependencies**
    Run the following commands to install the required PHP and Node.js packages:
    ```bash
    composer install
    npm install
    ```

3.  **Create Environment File**
    Copy the example environment file to create your local `.env` configuration:
    ```bash
    cp .env.example .env
    ```

4.  **Generate Application Key**
    Generate a unique application key for security:
    ```bash
    php artisan key:generate
    ```

5.  **Set Up Database Connection**
    Open the newly created `.env` file and update the following database connection details:
    ```env
    DB_DATABASE=laravel_db
    DB_USERNAME=root
    DB_PASSWORD=
    ```
    *(Adjust values as necessary for your local environment)*

6.  **Run Migration and Seeders**
    Execute the migrations to create the database tables and run the seeders to populate initial data:
    ```bash
    php artisan migrate --seed
    ```

7.  **Start Development Server**
    Start the local development server:
    ```bash
    php artisan serve
    ```

8.  **Access the Application**
    Open your browser and navigate to the following URL to access the application:
    [http://localhost:8000](http://localhost:8000)
