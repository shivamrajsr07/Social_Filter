# Social_Filter

Social_Filter is a simple PHP-MySQL web application that filters social media content based on a child's age. It includes a content submission form, age-based filtering, and a clean Bootstrap UI. This project demonstrates database connectivity, form handling, and content retrieval using PHP and MySQL.

---

## 🚀 Features

- Add social media content through a professional form  
- Save content in MySQL database  
- Filter content by child age groups  
- Display safe and age-appropriate items  
- Clean and simple Bootstrap UI  
- Fully PHP-based backend with MySQL integration  

---

## 📁 Project Structure

Assignment2/
│
├─ index.php # Add content form
├─ submit.php # Inserts content into DB
├─ display.php # Shows filtered results
├─ filter.php # Age selection page
├─ config.php # DB connection
│
├─ database/
│ └─ schema.sql # MySQL table structure
│
├─ assets/
│ ├─ css/
│ │ └─ style.css # Custom design
│ └─ js/
│ └─ script.js
│
└─ vendor/ # Optional (Bootstrap CDN)

yaml
Copy code

---

## 🗄 Database Setup

Create a database:

```sql
CREATE DATABASE content_filter_db;
Create the table using:

sql
Copy code
CREATE TABLE content_data (
    id INT AUTO_INCREMENT PRIMARY KEY,
    title VARCHAR(255) NOT NULL,
    description TEXT NOT NULL,
    category VARCHAR(50) NOT NULL,
    age_group VARCHAR(50) NOT NULL,
    content_url VARCHAR(255),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
🛠 Installation & Running the Project
1. Install PHP 8.3 (Thread Safe)
2. Install MySQL / XAMPP / WAMP
3. Start PHP server:
sh
Copy code
cd Assignment2
php -S localhost:8000
4. Open the project:
bash
Copy code
http://localhost:8000/index.php
🧪 Pages Overview
/index.php — Add new content

/filter.php — Select age group

/display.php — Shows filtered content

🤝 Contribution
Feel free to fork this project and improve it.

📜 License
This project is created for educational purposes. Free to use and modify.
