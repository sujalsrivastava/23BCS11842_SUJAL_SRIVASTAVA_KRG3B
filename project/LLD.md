# Low-Level Design (LLD)

## 📌 Overview
This document explains the internal structure of frontend and backend.

---

## 🧩 Frontend (React)

### Folder Structure
- src/components → reusable UI components
- src/pages → main screens
- src/api → API calls
- src/store → state management

### Key Files
- App.jsx → main component
- main.jsx → entry point

---

## 🔌 Backend (Spring Boot)

### Layers

#### Controller Layer
- Handles HTTP requests
- Example:
  - /api/items
  - /api/users

#### Service Layer
- Business logic
- Processes data before sending to DB

#### Repository Layer
- Uses JPA/Hibernate
- Communicates with database

---

## 🗄️ Database Design

### Example Entity: User
- id (Primary Key)
- name
- email
- password

### Example Entity: Item
- id
- name
- description
- created_at

---

## 🔁 Data Flow
Client → Controller → Service → Repository → Database → Response

---

## 🔐 Authentication (if implemented)
- JWT-based authentication
- Login / Signup APIs
