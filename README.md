# Item Management REST API – Spring Boot Application

## 1. Introduction
This project is a simple Java backend application developed using **Spring Boot**.  
It provides a **RESTful API** to manage a collection of items, similar to systems used in **e-commerce platforms (Flipkart)** or **media platforms (Netflix)**.

The application is intentionally kept simple and uses **in-memory data storage (ArrayList)** instead of a database, as required in the task description.

---

## 2. Objective of the Project
The main objective of this project is to:
- Demonstrate REST API development using Java and Spring Boot
- Implement basic CRUD-style operations (Add & Fetch)
- Apply input validation
- Follow clean coding and RESTful design principles
- Provide proper documentation and a deployable backend service

---

## 3. Technologies Used
- **Java 17**
- **Spring Boot**
- **Spring Web** (for REST APIs)
- **Jakarta Bean Validation** (for input validation)
- **Maven** (build and dependency management)

## 4. Item Model
The `Item` class represents the data model of the application.

### Fields:
- `id` – Unique identifier for the item
- `name` – Name of the item (required)
- `description` – Description of the item (required)
- `price` – Price of the item

### Validation:
- `name` and `description` are mandatory
- Validation is enforced using **Bean Validation annotations**

---

## 5. In-Memory Data Storage
- The application uses an **ArrayList** to store items
- Data is stored in memory only
- No database is used
- Data will be lost when the application restarts

---

## 6. REST API Endpoints

### 6.1 Add a New Item
**HTTP Method:** POST  
**Endpoint:** `/api/items`

**Request Body (JSON):**
```json
{
  "id": 1,
  "name": "Laptop",
  "description": "Gaming laptop",
  "price": 75000
}


Author By:- Vaishnavi Pagar
