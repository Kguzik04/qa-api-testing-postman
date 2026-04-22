# QA API Testing – Postman Project

## 📌 Overview

This project contains API tests created in **Postman** for a public REST API (JSONPlaceholder). The tests verify basic HTTP requests and responses to ensure correct API behavior.

The project demonstrates fundamental skills in API testing, including sending requests and validating responses.

---

## 🧪 Tested API

The tests are based on the public API:

[https://jsonplaceholder.typicode.com/](https://jsonplaceholder.typicode.com/)

This is a free fake REST API used for testing and learning purposes.

---

## 📂 Project Structure

```
qa-api-testing-postman/
│
├── collections/
│   └── Postman collection file
│
├── environments/
│   └── Postman environment file
│
└── README.md
```

---

## ✅ Covered Test Scenarios

### GET Requests

* Retrieve all posts
* Retrieve a single post by ID
* Validate response status code
* Validate response body structure

### POST Requests

* Create a new post
* Validate response status code
* Validate returned data

### PUT Requests

* Update an existing post
* Validate response status code

### DELETE Requests

* Delete a post
* Validate response status code

---

## 🧪 Example Test Script (Postman)

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Response contains data", function () {
    const jsonData = pm.response.json();
    pm.expect(jsonData).to.be.an("object");
});
```

---

## ⚙️ How to Run

1. Open Postman
2. Import the collection file
3. Import the environment file
4. Run the collection using Collection Runner

---

## 👤 Author

GitHub: [https://github.com/Kguzik04](https://github.com/Kguzik04)
