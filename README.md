# Employee Management REST API (Spring Boot)

This is a Spring Boot project designed to perform CRUD (Create, Read, Update, Delete) operations on an `employee` table using a REST API. The project connects to a MySQL database using both JPA and JDBC for data persistence.

---

## Features

The API allows you to perform the following operations on the `employee` table:

1. **Get all employees**  
   **Method:** `GET`  
   **Endpoint:** `/allemp`  
   Fetches the list of all employees.

2. **Get employee by ID**  
   **Method:** `GET`  
   **Endpoint:** `/emp/{empId}`  
   Fetches the details of a specific employee by their `empId`.

3. **Add a new employee**  
   **Method:** `POST`  
   **Endpoint:** `/emp`  
   **Request Body Example:**
   ```json
   {
     "empId": 5,
     "name": "E",
     "department": "HR",
     "salary": 60000
   }
4. **Delete an employee:**  
   **Method:** `DELETE`  
   **Endpoint:** `/emp/{empId}`  
  Deletes an employee by their `empId`.
5. **Update an employee:**  
   **Method:** `PUT`  
   **Endpoint:** `emp`  
    **Request Body Example:**
   ```json
   {
     "empId": 5,
     "name": "E",
     "department": "HR",
     "salary": 60000
   }
  ## Technologies Used 
  1. **Java:** The primary language used to build the application.
  2. **Spring Boot:** To create a RESTful web service.
  3. **JPA (Java Persistence API):** For ORM (Object-Relational Mapping) to handle database operations.
  4. **JDBC (Java Database Connectivity):** To connect with the MySQL database and perform raw SQL queries.
  5. **MySQL:** Database used to store employee data.
  ## Prerequisites
  Before running the project, ensure you have the following installed:
  1. **Java 8 or Later**
  2. **Maven** (for building project)
  3. **MySQL** (for the database)
