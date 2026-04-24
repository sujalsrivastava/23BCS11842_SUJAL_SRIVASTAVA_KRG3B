# Scaling Strategy

## Horizontal Scaling
- Multiple instances of services
- Load balancer distributes traffic

## Database Scaling
- Read replicas
- Sharding (for large data)

## Caching
- Redis for:
  - Search results
  - Session storage

## Async Processing
- Use queues for:
  - Notifications
  - CDC pipeline

## ElasticSearch
- Used for fast search
- Avoids DB load

## Rate Limiting
- Prevents abuse

## CDN
- For images (Cloudinary)

## Fault Tolerance
- Retry mechanisms
- Circuit breakers
