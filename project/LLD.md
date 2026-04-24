# Low Level Design (LLD)

## User Service
### APIs
- Register User
- Login User (JWT)

### Schema
User:
- user_id
- name
- email
- password_hash

---

## Listing Service
### Schema
Listing:
- listing_id
- name
- description
- location
- price
- images
- user_id

---

## Review Service
### Schema
Review:
- review_id
- listing_id
- user_id
- rating
- comment

---

## Booking Service
### Logic
1. Check availability
2. Lock using Redis
3. Process payment
4. Confirm booking

---

## Search Service
- Queries ElasticSearch
- Returns listing IDs

---

## CDC Pipeline
- DB → Connector → Streaming → ElasticSearch
