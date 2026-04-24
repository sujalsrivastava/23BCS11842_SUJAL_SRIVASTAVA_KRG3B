# API Documentation

## Auth APIs

### Register
POST /api/register
Body:
{
  "name": "user",
  "email": "user@mail.com",
  "password": "1234"
}

---

### Login
POST /api/login

Response:
{
  "token": "JWT_TOKEN"
}

---

## Listing APIs

### Add Listing
POST /api/listings

### Get Listing
GET /api/listings/{id}

---

## Search API
GET /api/search?q=location

---

## Review API
POST /api/review

---

## Booking API
POST /api/book

---

## Notification
Triggered internally after booking
