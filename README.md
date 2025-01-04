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

## **Setup**

### **Prerequisites**
- Python 3.8 or above installed.
- Postman installed for testing.

### **Installation**
1. Clone this repository to your local machine:
   ```bash
   git clone <repository_url>
   cd Library-Management-System
Install dependencies using:

bash
Copy code
pip install -r requirements.txt
Run the Flask app:

bash
Copy code
python app.py
The app will start running on http://127.0.0.1:5000.

Using Postman for API Testing
Base URL
For local testing, the base URL is:

arduino
Copy code
http://127.0.0.1:5000
Replace <base_url> in the endpoints below with this base URL.

Endpoints
Books Endpoints
Create a Book

URL: <base_url>/books
Method: POST
Headers:
bash
Copy code
Content-Type: application/json
Body (JSON):
json
Copy code
{
    "title": "The Great Gatsby",
    "author": "F. Scott Fitzgerald"
}
Response:
json
Copy code
{
    "id": 1,
    "title": "The Great Gatsby",
    "author": "F. Scott Fitzgerald",
    "available": true
}
Get All Books

URL: <base_url>/books
Method: GET
Response:
json
Copy code
[
    {
        "id": 1,
        "title": "The Great Gatsby",
        "author": "F. Scott Fitzgerald",
        "available": true
    }
]
Get a Book by ID

URL: <base_url>/books/<id>
Method: GET
Example: <base_url>/books/1
Response:
json
Copy code
{
    "id": 1,
    "title": "The Great Gatsby",
    "author": "F. Scott Fitzgerald",
    "available": true
}
Update a Book

URL: <base_url>/books/<id>
Method: PUT
Headers:
bash
Copy code
Content-Type: application/json
Body (JSON):
json
Copy code
{
    "title": "The Great Gatsby (Updated)"
}
Response:
json
Copy code
{
    "id": 1,
    "title": "The Great Gatsby (Updated)",
    "author": "F. Scott Fitzgerald",
    "available": true
}
Delete a Book

URL: <base_url>/books/<id>
Method: DELETE
Response:
json
Copy code
{
    "message": "Book deleted successfully"
}
Members Endpoints
Create a Member

URL: <base_url>/members
Method: POST
Headers:
bash
Copy code
Content-Type: application/json
Body (JSON):
json
Copy code
{
    "name": "John Doe",
    "email": "john.doe@example.com"
}
Response:
json
Copy code
{
    "id": 1,
    "name": "John Doe",
    "email": "john.doe@example.com"
}
Get All Members

URL: <base_url>/members
Method: GET
Response:
json
Copy code
[
    {
        "id": 1,
        "name": "John Doe",
        "email": "john.doe@example.com"
    }
]
Get a Member by ID

URL: <base_url>/members/<id>
Method: GET
Example: <base_url>/members/1
Response:
json
Copy code
{
    "id": 1,
    "name": "John Doe",
    "email": "john.doe@example.com"
}
Update a Member

URL: <base_url>/members/<id>
Method: PUT
Headers:
bash
Copy code
Content-Type: application/json
Body (JSON):
json
Copy code
{
    "name": "Johnathan Doe"
}
Response:
json
Copy code
{
    "id": 1,
    "name": "Johnathan Doe",
    "email": "john.doe@example.com"
}
Delete a Member

URL: <base_url>/members/<id>
Method: DELETE
Response:
json
Copy code
{
    "message": "Member deleted successfully"
}
Assumptions
Data is stored in memory, so all records will reset after restarting the app.
No authentication or authorization is implemented.
Basic error handling assumes valid inputs and endpoint usage.
Limitations
Data is not persisted (no database used).
Minimal input validation.
API is designed for educational purposes and not production use.
License
This project is open-source and available for educational purposes.

csharp
Copy code

You can directly paste this content into your **README.md** file in the GitHub repository.







