# 📚 Postman API Testing Project – Simple Books API

## 📌 Project Overview
This project demonstrates API testing using Postman on a RESTful Simple Books API.  
It covers CRUD operations, authentication handling, query parameters, path variables, and basic automated test scripts using JavaScript assertions in Postman.

The goal of this project was to understand how APIs work and how to test them effectively using Postman.

---

## 🚀 Features Implemented

### ✅ HTTP Methods Covered
- GET – Retrieve list of books
- GET – Retrieve single book using path variable
- GET – Retrieve books with query parameters (limit, type)
- POST – Create new order (Authentication required)
- PATCH – Update an existing order
- DELETE – Delete an order

---

## 🔐 Authentication
- Used access token generation for protected endpoints
- Implemented token-based authentication in request headers

---

## 🧪 API Testing Performed

### ✔ Status Code Validation
- 200 OK
- 201 Created
- 400 Bad Request
- 404 Not Found

### ✔ Response Body Validation
- Checked required properties in JSON response
- Verified stock availability
- Validated order creation response

### ✔ Query Parameters Testing
- Used `limit` parameter
- Tested optional and mandatory parameters
- Verified behavior for invalid values

### ✔ Path Variables
- Implemented dynamic path variables (e.g. `/books/:bookId`)

---

## 🔄 Variables Used

- Collection Variables (`baseUrl`)
- Global Variables (`bookId`, `orderId`)
- Extracted response data and reused in subsequent requests

Example:
```javascript
let response = pm.response.json();
pm.globals.set("bookId", response[0].id);
```

---

## 🛠 Tools & Technologies

- Postman
- REST API
- JavaScript (basic test scripting)
- JSON
- Chai Assertion Library (Postman built-in)

---

## 📂 Project Structure

```
postman-api-testing-project/
│
├── SimpleBooksAPI.postman_collection.json
├── simple-books-api.md
└── README.md
```

---

## 📈 Learning Outcomes

Through this project, I learned:

- How REST APIs work
- Structure of HTTP request & response
- Authentication using access tokens
- Writing basic API tests in Postman
- Using variables to chain requests
- Handling different HTTP status codes

---

## ▶ How to Run This Project

1. Install Postman (Desktop or Web)
2. Import the `SimpleBooksAPI.postman_collection.json` file
3. Set the `baseUrl` collection variable
4. Run requests individually or using Collection Runner

---

## 📌 Future Improvements

- Add advanced automated test scenarios
- Integrate Newman for CLI execution
- Add CI/CD pipeline integration
- Generate automated test reports

---

## 👤 Author

Anugrah Deolia

---
