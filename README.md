# 📘 Simple Books API Testing – Postman Collection

This repository contains a complete Postman collection for testing the [Simple Books API](https://simple-books-api.glitch.me), designed to demonstrate API testing concepts such as authentication, CRUD operations, variable usage, scripting, and assertions.

## 📌 Project Overview

The **Simple Books API Testing** collection showcases essential API test cases including:

- Retrieving all books
- Authenticating a user
- Placing, updating, and deleting book orders
- Validating response status codes and payloads
- Using environment and global variables
- Pre-request and test scripts for data-driven testing

## 🧰 Tools Used

- **Postman** – API testing platform   
- **JavaScript (Chai)** – For test assertions in Postman scripts  

## 📂 Collection Details

| Request Name                     | Method | Description                         |
|----------------------------------|--------|-------------------------------------|
| LIST_OF_ALL_BOOKS               | GET    | Retrieves all available books       |
| Authentication                  | POST   | Generates a bearer token            |
| PLACE_ORDER                     | POST   | Places a new book order             |
| GET_ORDER_DETAILS               | GET    | Retrieves order details by ID       |
| UPDATE_ORDER                    | PATCH  | Updates customer name in an order   |
| DELETE_ORDER                    | DELETE | Deletes an order by ID              |
| RANDOM_DATA_PARSE_JSON_RESPONSE| POST   | Places order using random data with status validation |
| SET_RESET_VALUE                 | POST   | Demonstrates use of variables reset |

## 🧪 Test Scripts Highlights

- ✅ **Positive Test Cases**: Valid order placements and successful retrievals
- ❌ **Negative/Deliberate Failures**: Simulates expected failures (e.g., 404 responses)
- 🔁 **Dynamic Variables**: Use of `pm.variables.set()` for dynamic customer names
- 🔍 **Assertions**: Includes Chai assertions for status code and response content validation

## ▶️ How to Use

1. **Import the Collection**
   - Open Postman
   - Click **Import** > Upload `Simple Books API Testing.postman_collection.json`

2. **Set Up Environment**
   - Create a new environment with variable:
     - `base_url = https://simple-books-api.glitch.me`

3. **Run Tests**
   - Use **Collection Runner** or individual requests
   - Observe console and test tab for assertion results



