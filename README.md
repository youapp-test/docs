# Project README

## Overview:
This project comprises three main services:
- **auth-service**: Handles user authorization.
- **profile-service**: Manages user details/profiles.
- **chat-service**: Facilitates chat functionalities.

## Features:
- **auth-service**: 
    - Responsible for user authorization.
- **profile-service**: 
    - Manages user details and profiles.
- **chat-service**: 
    - Provides chat functionalities.

## Integration:
- **auth-service**: 
    - Integrates with other services for user authentication.
- **profile-service** and **chat-service**: 
    - Utilize auth local strategy for authentication.
    - In case of auth-service downtime, both profile-service and chat-service remain functional.
    - Auth local strategy employs RabbitMQ as a message broker for seamless communication.
    - Scalable: Can handle heavy loads efficiently by distributing tasks across multiple services.

## Dependencies:
- Nest.js
- RabbitMQ
