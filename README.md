# 📚LIBRARY MANAGEMENT SYSTEM 
# 📑Description / Overview 
This Laravel-based CRUD MVC web application was created to efficiently manage library resources, including books, members, and borrowing/returning transactions. It was developed as part of the Midterm Examination for the IT course in SYSTEM INTEGRATION.
# 🔖Objectives
The Library Management System enables administrators and librarians to easily add, view, edit, and remove records while also tracking book borrowing and return activities. It is built using the Model-View-Controller (MVC) design pattern to ensure a well-structured and maintainable system.
## ✨ Features / Functionality
* **Book Management:** Add, edit, delete, and view detailed book information (CRUD operations).
* **Member Management:** Manage member records, including students, teachers, and other users.
* **Search & Filtering:** Users can search and filter books quickly for easier access.
* **User Interface:** Features a responsive and user-friendly interface built with Laravel's Blade templates.
* **Setup:** Supports database migration and seeding for smooth initial setup and deployment.
  
* **Model (M)**
    -Book.php
    -Borrowing.php
    -Students.php
    -User.php
 * **View (V)**
    -resources/views/books/index.blade.php
    -resources/views/books/create.blade.php
    --resources/views/books/show.blade.php
 * **Controller (C)**
    -BookController.php
    -BorrowingController.php
    -Controller.php
    -StudentController.php
    
## ⚙️CRUD Operations
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
    ```bash
    composer install
    npm install
    ```
3.  **Create Environment File**
    ```bash
    cp .env.example .env
    ```
4.  **Generate Application Key**
    ```bash
    php artisan key:generate
    ```
5.  **Set Up Database Connection**
    ```env
    DB_DATABASE=laravel_db
    DB_USERNAME=root
    DB_PASSWORD=
    ```
6.  **Run Migration and Seeders**
    ```bash
    php artisan migrate --seed
    ```
7.  **Start Development Server**
    ```bash
    php artisan serve
    ```
8.  **Access the Application**
    [http://localhost:8000](http://localhost:8000)
