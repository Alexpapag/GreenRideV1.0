# GreenRide - Carpooling Platform

Distributed system for ride sharing between students.

## Description

GreenRide is a web application that allows users to create and book seats in shared rides (carpooling), reducing transportation costs and environmental impact.

## Features

- Authentication & Authorization (JWT for API, Session-based for UI)
- Ride Management (create, search, update rides)
- Booking System with real-time availability checking
- User Roles (Driver, Passenger, Admin)
- External Service Integration (geolocation for distance/duration)
- Admin Panel with statistics
- REST API with OpenAPI/Swagger documentation

## Technologies

Backend: Spring Boot 3.x, Spring Security, Spring Data JPA
Frontend: Thymeleaf, HTML, CSS, JavaScript
Database: H2 (development) / PostgreSQL (production)
API: REST, JWT Authentication
Documentation: Swagger/OpenAPI

## Requirements

- Java 17+
- Maven 3.6+

## Installation & Execution

Clone repository:
git clone https://github.com/Alexpapag/GreenRide.git
cd GreenRide

Build and run:
mvn spring-boot:run

Application available at: http://localhost:8080/web/auth/login

## API Documentation

Swagger UI: http://localhost:8080/swagger-ui.html
OpenAPI JSON: http://localhost:8080/v3/api-docs
Postman Collection: /docs/postman/

## Test Credentials

User: maria / maria123
Admin: admin / admin123

## Project Structure

src/main/java/com/greenride/
- controller/       REST & MVC Controllers
- service/          Business Logic
- repository/       Data Access Layer
- entity/           JPA Entities
- dto/              Data Transfer Objects
- config/           Security & Configuration
- exception/        Exception Handling

src/main/resources/
- templates/        Thymeleaf Templates
- static/           CSS, JS, Images
- application.properties

## Main Endpoints

Authentication:
POST /api/auth/register - User registration
POST /api/auth/login - Login (returns JWT)

Rides:
GET /api/rides - Search rides
POST /api/rides - Create ride
GET /api/rides/{id} - Ride details

Bookings:
POST /api/bookings - Book seats
GET /api/bookings/my-bookings - My bookings

## Development Team

Vasileios Gkoumas - it2021020
Alexandros Papageorgiou - it2021072
Alexandros Kostakis  - it2021147

