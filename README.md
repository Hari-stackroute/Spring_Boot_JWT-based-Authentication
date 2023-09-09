# Spring Boot JWT Authentication

This Spring Boot project implements JWT authentication for securing APIs using JSON Web Tokens (JWT). It allows you to authenticate and authorize users efficiently.

## Stack

- Java 8
- Spring Boot
- MySQL
- JWT
- Swagger 2

## How JWT Authentication Works

1. Users log in and receive an Access Token.
2. Access Tokens are sent with requests to protected endpoints.
3. The server validates Access Tokens, granting access if valid.

## Implementation Highlights

- `JwtTokenFilter`: Validates and extracts JWT from requests.
- `JwtTokenProvider`: Manages JWT creation, validation, and authentication.
- `MyUserDetails`: Implements `UserDetailsService` for user data.
- `WebSecurityConfig`: Configures security settings and applies JWT authentication.

## Token-Generation Service Testing using Postman

![Token-Generation Service Testing using Postman](https://github.com/sanbit876/Spring_Boot_JWT-based-Authentication/assets/24634950/5da61e3c-5890-4eae-9fe5-193b86f1fc52)


## Getting Started

1. Clone the repository.
2. Install Java 8 and Maven.
3. Build and run the project: `mvn spring-boot:run`.
4. Access Swagger docs at `http://localhost:8080/swagger-ui.html`.
5. Use JWT for authentication by signing in at `/users/signin`.
