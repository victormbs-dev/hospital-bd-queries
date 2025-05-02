# Hospital Database SQL Queries

![Database](https://img.shields.io/badge/Database-SQL-blue) 
![License](https://img.shields.io/badge/License-MIT-green)

## 📌 Overview
A comprehensive collection of SQL queries for hospital database management, covering patient records, admissions, and reporting.

## 📂 Repository Structure
/hospital-db-queries/

│── /basic-queries/

│── /advanced-queries/

│── /data-modification/

│── LICENSE

└── README.md


## 🛠️ Features
- **Patient Data Retrieval**
- **Admission Statistics**
- **Data Cleaning Operations**
- **Complex Joins & Aggregations**
- **NULL Value Handling**

## 🔍 Query Categories
🔹 Basic Retrieval
sql
SELECT first_name FROM patients WHERE height > 160;


🔹 Data Modification
sql
UPDATE patients SET allergies = 'NKA' WHERE allergies IS NULL;


🔹 Advanced Analytics
sql
SELECT province_name, COUNT(*) 
FROM patients
JOIN province_names ON patients.province_id = province_names.province_id
GROUP BY province_name;
