# 🚗 Sunless Express

**Sunless Express** is a simple and intuitive carpooling web application designed to connect drivers and passengers. This project was developed as part of the "Digital Development" academic module.

## 📋 Features

### 🔐 Authentication (Single Page Interface)
- **Login & Sign Up** combined on a single page with smooth transitions handled by JavaScript (no page reload required).
- Secure PHP session management.
- Password hashing (`password_hash`) for enhanced security.

### 🔍 Ride Search
- Multi-criteria search bar:
  - Departure City
  - Arrival City
  - Travel Date (Calendar selector)
- Dynamic result filtering via PHP/SQL.

### 🎨 User Interface (UI/UX)
- **Dark Mode** design with **Wine Red** accents.
- Clean, responsive layout.
- Interactive user feedback (JavaScript Alerts on action buttons).

## 🛠️ Tech Stack

* **Frontend:** HTML5, CSS3 (Flexbox, Design System), JavaScript (DOM Manipulation, Events).
* **Backend:** PHP 8 (Native).
* **Database:** MySQL.
* **Local Server:** Apache (via XAMPP).

## 🚀 Installation & Setup

Follow these steps to run the project locally on your machine.

### 1. Prerequisites
Ensure you have **XAMPP** (or WAMP/MAMP) installed to manage Apache and MySQL.

### 2. File Installation
1.  Clone this repository or download the files.
2.  Move the project folder into the XAMPP `htdocs` directory (usually `C:\xampp\htdocs\covoiturage`).

### 3. Database Configuration
1.  Open **phpMyAdmin** (`http://localhost/phpmyadmin`).
2.  Create a new database named **`covoiturage`**.
3.  Click on the **Import** tab and select the `table.sql` file provided in this project.
4.  Run the import to create the necessary tables (`utilisateurs`, `trajets`, etc.).

### 4. Running the App
1.  Open **XAMPP Control Panel** and start **Apache** and **MySQL**.
2.  Open your browser and navigate to:
    ```
    http://localhost/covoiturage/index.php
    ```

## 📂 Project Structure

```bash
├── index.php           # Home page and search results
├── auth.php            # Login and Registration page
├── auth_traitement.php # Backend logic (Login/Register processing)
├── style.css           # Stylesheet (Dark & Wine Red Theme)
├── index.js            # Frontend scripts for the Home page
├── auth.js             # Frontend scripts for Authentication toggles
├── logout.js           # Logout confirmation script
└── table.sql           # Database structure import file
