# HomeChef System

The HomeChef Booking System is a full-stack web application where users can register, browse chefs and menus, and make bookings. It is built using Spring Boot (backend) and React (frontend) with MySQL as the database.

<img width="1884" height="995" alt="home" src="https://github.com/user-attachments/assets/61909517-1c09-4da3-8515-50a998ba0083" />

<img width="1868" height="999" alt="menu" src="https://github.com/user-attachments/assets/882f1f98-d4b9-4d0c-a6f9-d6e5b346dbbd" />

<img width="1863" height="999" alt="admin" src="https://github.com/user-attachments/assets/2dd3a514-72a0-4591-b693-9c32fa1379a9" />


## Features

👤 User Management: Register, login, and authentication

👨‍🍳 Chef Management: Add chefs by Admin with details (name, specialty, experience, email)

🍽️ Menu Management: Admin can create menus with price and description

📅 Booking System: Users can book chefs and menus for specific cuisine

💳 Billing: Auto-generated billing with booking reference and status


## Project structure

**homechef-system/**
  - **backend/** – Spring Boot Project (STS)
    - `src/main/java/...` – Java source code  
    - `src/main/resources/` – application.properties  
    - `pom.xml` – Maven build file  
  - **frontend/** – React + Vite project
    - `src/` – React components & pages  
    - `public/` – Static assets  
    - `package.json` – npm dependencies  
    - `vite.config.js` – Vite configuration


## Database Design

## Entities

User(id, name, email, password)

Admin(id,name, email, password)

Chef(id, name, speciality, experience, email)

Menu(id, name, price, chef_id)

Booking(id, user_id, chef_id, menu_id, date)

Billing(id, booking_id, user_id, amount, status)

##  Tech Stack

## Backend

Spring Boot (REST API)

Spring Data JPA

MySQL (Database)

Maven (Build tool)

## Frontend

React.js

Axios (API calls)

Tailwind (Styling)

## Tools

Postman – API Testing

GitHub – Version Control

STS  – Backend Development

VS Code – Frontend Development

## How to Run

## Backend (Spring Boot)

Go to backend/ folder

Update application.properties with your MySQL credentials

run the application

## Frontend (visual studio)

1. Go to frontend/ folder

2. Install dependencies

          npm install


3. Start frontend

          npm run dev


Frontend will run on http://localhost:5173
Backend will run on http://localhost:8080

## Future Scope

Microservices architecture with Eureka & API Gateway

JWT authentication

Payment gateway integration (Razorpay/Stripe)

Docker & Kubernetes deployment

## References

References

Spring Boot Documentation

React Documentation

MySQL Documentation

Postman
