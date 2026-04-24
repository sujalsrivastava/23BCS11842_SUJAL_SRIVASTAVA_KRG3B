# API Documentation

## 📌 Base URL
http://localhost:8080/api

---

## 🔑 Authentication APIs

### POST /auth/register
Register a new user

### POST /auth/login
Login user

---

## 📦 Item APIs

### GET /items
Fetch all items

### GET /items/{id}
Fetch item by ID

### POST /items
Create new item

### PUT /items/{id}
Update item

### DELETE /items/{id}
Delete item

---

## 📌 Request Example
```json
{
  "name": "Item 1",
  "description": "Sample item"
}
