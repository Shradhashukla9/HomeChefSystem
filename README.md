# HomeChef System

The HomeChef Booking System is a full-stack web application where users can register, browse chefs and menus, and make bookings. It is built using Spring Boot (backend) and React (frontend) with MySQL as the database.

## Features

👤 User Management: Register, login, and authentication

👨‍🍳 Chef Management: Add chefs by Admin with details (name, specialty, experience, email)

🍽️ Menu Management: Admin can create menus with price and description

📅 Booking System: Users can book chefs and menus for specific cuisine

💳 Billing: Auto-generated billing with booking reference and status

##  Project Structure

homechef-system/
│── backend/                  # Spring Boot Project (STS)
│   ├── src/main/java/...     # Java source code
│   ├── src/main/resources/   # application.properties
│   └── pom.xml               # Maven build file
│
│── frontend/                 # React + Vite project
│   ├── src/                  # React components & pages
│   ├── public/               # Static assets
│   ├── package.json          # npm dependencies
│   └── vite.config.js        # Vite configuration
│
└── README.md


## Database Design

# Entities

User(id, name, email, password)

Admin(id,name, email, password)

Chef(id, name, speciality, experience, email)

Menu(id, name, price, chef_id)

Booking(id, user_id, chef_id, menu_id, date)

Billing(id, booking_id, user_id, amount, status)

##  Tech Stack

# Backend

Spring Boot (REST API)

Spring Data JPA

MySQL (Database)

Maven (Build tool)

# Frontend

React.js

Axios (API calls)

Tailwind (Styling)

# Tools

Postman – API Testing

GitHub – Version Control

STS  – Backend Development

VS Code – Frontend Development

## How to Run

# Backend (Spring Boot)

Go to backend/ folder

Update application.properties with your MySQL credentials

run the application

# Frontend (visual studio)

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