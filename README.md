# 📰 News Management System

A full-stack news management web application developed with **Pure PHP** and **MySQL** as part of a university project.

---

## 📚 Overview

This project is a simple yet powerful CMS (Content Management System) for managing news posts, authors, and categories.  
It supports user roles, authentication, secure session handling, and basic CRUD operations.

---

## ✨ Features

- User Authentication (Signup & Login with session management)
- Pending Authors system (approval required by Admin)
- Role-based Access Control:
  - **Admin**: Full access to posts, categories, authors, and pending authors
  - **Author**: Access to manage only their own posts
- Posts Management (Create, Read, Update, Delete)
- Categories Management (Add, Edit, Delete)
- Image Upload Handling for posts
- Search Functionality for posts
- Secure Login with password hashing
- Clean and organized project structure

---

## ⚙️ Technologies Used

- PHP (Pure)
- MySQL
- HTML5 / CSS3
- XAMPP (for local development server)

---

## 🛠️ Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/news-management-system.git
   ```

2. Move the project folder to your server root directory (for XAMPP, it's `htdocs/`).

3. Import the database:
   - Open **phpMyAdmin**.
   - Create a new database (e.g., `newsdb`).
   - Import the SQL file located at `/dataBase/news.sql`.

4. Configure the database connection:
   - Open `db.php` and update your database credentials:
     ```php
     $conn = new mysqli('localhost', 'root', '', 'newsdb');
     ```

5. Start Apache and MySQL using XAMPP.

6. Open your browser and navigate to:
   ```
   http://localhost/news-management-system/
   ```

---


## 🔐 Access Control

- **Admin** users can manage:
  - All posts
  - All categories
  - All authors
  - Pending authors
- **Author** users can:
  - Create, edit, and delete only their own posts
  - Cannot access authors list, pending authors, or category management pages
- Unauthorized access is prevented through session and role checks.

---

## 📌 Notes

- Passwords are stored securely using PHP `password_hash()` and verified using `password_verify()`.
- Role management is handled through simple `role` fields inside the database.
- Proper redirecting is implemented for unauthorized access attempts.
- File uploads (post images) are stored inside the `/uploads/` directory.

---

## 🧑‍💻 Developer

- **Name**: [Ihab Taysir]
- **LinkedIn**: [www.linkedin.com/in/ihab-taysir-8a0695250]
- **Email**: [tihab215@gmail.com]

---

# 🚀 Thank you for checking out this project!
