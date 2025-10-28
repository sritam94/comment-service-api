Comment-Service-API

Comment Management Microservice – Spring Boot 3.x, PostgreSQL & Redis Caching

Overview

Comment-Service-API is a standalone microservice designed for managing user comments in applications (blogs, product reviews, social feeds). Built for scalability, security, and performance, it features caching via Redis and clean architecture.

Features

Endpoints for creating, retrieving, updating, deleting comments

PostgreSQL storage with schema optimised for search and filtering

Redis cache integration for frequently accessed comment lists

Rate limiting and anti-spam checks to secure backend from misuse

Comprehensive documentation (Swagger/OpenAPI) for frontend integration

Dockerised microservice for easy deployment

Technology Stack

Java 17

Spring Boot 3.x

PostgreSQL

Redis

JPA / Hibernate

Spring Security (token-based)

Docker

GitHub Actions

Architecture Diagram

Setup Guide

Clone the repo

Setup PostgreSQL and Redis locally or via Docker

Configure application.yml with DB and Redis settings

Build & run:

docker build -t comment-service-api .  
docker run -p 8081:8081 comment-service-api  


Access API docs: http://localhost:8081/swagger-ui.html

Example Endpoints

POST /api/v1/comments — submit a new comment

GET /api/v1/comments?postId=123&page=0 — get comments for a post

PUT /api/v1/comments/{id} — update comment

DELETE /api/v1/comments/{id} — delete comment

What I Contributed

Designed DB schema for efficient filtering by postId, time, user

Implemented Redis caching for hot-comment lists

Introduced rate limiting and anti-spam verification steps

Authenticated endpoints via token & role controls

Documented all APIs in Swagger for developer handover
