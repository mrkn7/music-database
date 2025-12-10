# 🎵 The Music Box Project (STAT 311 Recitation 9)

**Course:** STAT 311 - Modern Database Systems  
**Recitation:** 9 - Object-Relational Database & XML Simulation  
**Institution:** Middle East Technical University (ODTÜ)

---

## 📖 Overview

This project is a web-based simulation designed to demonstrate **Object-Relational Database (ORDBMS)** concepts and **XML Data Processing** in a client-side environment. 

Since the course environment restricts server-side execution (PHP/SQL), this application simulates a full-stack database interaction using **JavaScript (ES6)**, **Fetch API**, and **DOM Manipulation**. It processes raw CSV data, transforms it into an XML structure, and maps it to Object-Oriented classes.

### 🚀 Live Demo
[Click here to view the project](https://mrkn7.github.io/music-database/)  
*(Note: Ensure your repository is deployed to GitHub Pages for this link to work)*

---

## 🎯 Key Concepts Covered

This project bridges theory and practice based on the lecture notes:

### 1. Web Database Simulation (Chapter 11)
- Simulates server-side logic purely on the client side.
- Uses **Fetch API** to retrieve data from a local file system (`data/best_selling_artists.csv`) mimicking a database query.
- Bypasses **CORS (Cross-Origin Resource Sharing)** restrictions using a local server environment.

### 2. Object-Relational Modeling (Chapter 12)
- Implements **Object-Oriented Programming (OOP)** to manage data.
- **Encapsulation:** Data and behavior (e.g., `getPhotoUrl()`) are bundled within the `Artist` class.
- **Inheritance & Polymorphism:**
  - `Band` class extends `Artist`.
  - `SoloArtist` class extends `Artist`.
  - The UI adapts dynamically based on whether the object is a Band or a Solo Artist.

### 3. XML & Data Transformation (Chapter 13)
- **ETL Pipeline:** Implements a runtime "Extract-Transform-Load" process.
- **Data Cleaning:** Sanitizes dirty data (e.g., fixing malformed sales figures).
- **XML Parsing:** Converts flat CSV data into a hierarchical **XML DOM Tree**, handling special characters (e.g., escaping `&` in "R&B").

---

## 📂 Folder Structure

```text
music-database/
│
├── index.html                 # Main application logic (HTML/CSS/JS)
│
├── data/
│   └── best_selling_artists.csv  # Raw Dataset (Source: Kaggle)
│
├── images/
│   ├── 1.jpg                  # Images mapped by Object ID
│   ├── 2.jpg
│   └── ... 
│
└── README.md                  # Project Documentation
