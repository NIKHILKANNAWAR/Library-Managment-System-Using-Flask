# **Library Management System API**

This project implements a Flask-based REST API for managing a library system. It allows users to perform CRUD (Create, Read, Update, Delete) operations on books and members. The API is tested using Postman.

---

## **Features**

### **Books API:**
- Add a book
- View all books
- Get a specific book by its ID
- Update a book
- Delete a book

### **Members API:**
- Add a member
- View all members
- Get a specific member by their ID
- Update a member
- Delete a member

---

# **Using Postman for API Testing**

### **Base URL**
For local testing, the base URL is:

http://127.0.0.1:5000


Replace `<base_url>` in the endpoints below with this base URL.

### **Books Endpoints**

**2. Get All Books**

- **URL:** `<base_url>/books`
- **Method:** GET

**3. Get a Book by ID**

- **URL:** `<base_url>/books/<id>`
- **Method:** GET
- **Example:** `<base_url>/books/1`

**4. Update a Book**

- **URL:** `<base_url>/books/<id>`
- **Method:** PUT
- **Headers:**
  - Content-Type: application/json
- **Body (JSON):**
  ```json
  {
    "title": "The Great Gatsby (Updated)"
  }

**5. Delete a Book**

- **URL:** `<base_url>/books/<id>`
- **Method:** DELETE

### **Members Endpoints**

**1. Create a Member**

- **URL:** `<base_url>/members`
- **Method:** POST
- **Headers:**
  - Content-Type: application/json
- **Body (JSON):**
  ```json
  {
    "name": "John Doe",
    "email": "john.doe@example.com"
  }

  **2. Get All Members**

- **URL:** `<base_url>/members`
- **Method:** GET

**3. Get a Member by ID**

- **URL:** `<base_url>/members/<id>`
- **Method:** GET
- **Example:** `<base_url>/members/1`

**4. Update a Member**

- **URL:** `<base_url>/members/<id>`
- **Method:** PUT
- **Headers:**
  - Content-Type: application/json
- **Body (JSON):**
  ```json
  {
    "name": "Johnathan Doe"
  }

  **5. Delete a Member**

- **URL:** `<base_url>/members/<id>`
- **Method:** DELETE
