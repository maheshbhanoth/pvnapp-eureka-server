# PVNApp Eureka Server

This project is a **Spring Cloud Netflix Eureka Server** that provides service discovery for the PVNApp microservices ecosystem.  
It acts as a registry where all microservices can register themselves and discover other services without hardcoding hostnames or ports.

## Features
- Service registration and discovery
- Eliminates the need for hardcoded service URLs
- Supports client-side load balancing (with Spring Cloud + Ribbon/Feign)
- Web dashboard to view registered services

## Tech Stack
- Java 17+
- Spring Boot
- Spring Cloud Netflix Eureka

## How It Works
1. Eureka Server starts and listens for service registrations.
2. Microservices (like `student-service`, `auth-service` etc..) register with Eureka using their application name.
3. Other services can discover them using the Eureka registry instead of static URLs.

## Running the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/maheshbhanoth/pvnapp-eureka-server.git
