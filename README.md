# Facial Recognition Attendance System

This is a Flask-based Facial Recognition Attendance System that stores student face data and tracks attendance by recognizing the faces from an uploaded image of present students.

> 🧠 This was my very first full-stack project — built with zero prior experience in web development or Flask and most importantly without any AI ! While the codebase is messy and lacks proper structure, security, and error handling, it was a great learning experience and actually works pretty well!

---

## ✨ Features

- Add new students and capture their face data
- Mark attendance via uploaded image
- Store attendance records in a database
- Basic web interface built using Flask templates

---

## 🚀 Getting Started

Follow these steps to run the project locally:

### 🔧 Prerequisites

Make sure you have the following installed:

- Python 3.7+ (Recommended - 3.12.10)
- `pip` package manager (Recommended version - 24.3.1)

The included libraries in project uses Dlib in background which works best with the recommended versions of Python and pip !!

### 📁 Clone the Repository

```bash
git clone https://github.com/harshil-mistry/facial-attendance.git
cd facial-attendance
```

### 🛠️ Create a Virtual Environment (Optional but Recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 📦 Install Dependencies
```bash
pip install -r requirements.txt
```


### 🛢️ Setting Up the Database (Using XAMPP)

This project uses **MySQL** for storing student and attendance records. Here's how to set it up using XAMPP:

### 🔧 Step-by-Step Guide

1. **Start XAMPP**  
   - Open the XAMPP Control Panel.
   - Start **Apache** and **MySQL** modules.

2. **Open phpMyAdmin**  
   - Visit [http://localhost/phpmyadmin](http://localhost/phpmyadmin)

3. **Create a New Database**  
   - Click on **"New"** in the left sidebar.
   - Name the database `attendance` and click **"Create"**.

4. **Import the SQL File**
   - Inside phpMyAdmin, select your new database.
   - Click on the **"Import"** tab.
   - Choose the `attendance.sql` file included in the `Database` Folder.
   - Click **"Go"** to import all tables.


Now your MySQL database is ready and you can run the Flask app! ✅


### ✅ Running the App
```bash
python attendance.py
```

### 🧠 Disclaimer
1. After running the app, the credentials for logging in are
   - Username  : admin1
   - Password : password

    Btw, these cerdentials are hardcored in the code :) Ik dumb but was a newbie back then and too lazy to improve the code RN. 

2. After logging in, first add some students data in the database with individual students image.

3. Then you can try marking attendance, and upload an image with multiple faces.

4. If you try marking attendance without adding students data first, you'll likely encounter an error, hehe. So remember to add data and then mark attendance. 👍

>This project is a beginner-level prototype. It’s not production-ready, but a good stepping stone for learning Flask, OpenCV, and machine learning concepts.
Feel free to explore, modify, and build upon it — and laugh at my beginner code if you must! 😄
