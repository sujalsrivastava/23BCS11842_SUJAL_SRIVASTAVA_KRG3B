# High Level Design (HLD)

## Overview
This system is a scalable hotel rental / listing platform where users can:
- Search listings
- Add listings
- Book hotels
- Add reviews

## Architecture Components

### 1. API Gateway + Load Balancer
- Handles authentication, authorization
- Routes requests to services
- Rate limiting

### 2. User Service
- User registration & login
- JWT-based session management

### 3. Search Service
- Handles search queries
- Uses ElasticSearch for fast retrieval

### 4. Listing Service
- Add/View listings
- Stores data in Listing DB

### 5. Review Service
- Users can add reviews
- Stored in Review DB

### 6. Booking + Checkout Service
- Handles booking flow
- Uses Redis locking to prevent double booking

### 7. Notification Service
- Sends booking confirmation
- Uses FCM/APNS

### 8. CDC Pipeline
- Syncs DB changes to ElasticSearch
- Uses streaming service

### 9. Third Party Services
- Mapbox (location services)
- Cloudinary (image storage)

## Databases
- MongoDB (Listings, Users)
- ElasticSearch (Search)
- Redis (Locking, Cache)

## Flow
Client → API Gateway → Services → DB/Cache → Response
