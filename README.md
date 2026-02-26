# 🏨 Hotel Booking System (Full-Stack)

An enterprise-grade full-stack hotel reservation platform built using **Spring Boot (Backend)** and **React.js (Frontend)**.  
The system allows users to browse hotels, check room availability, apply promotions, and securely book rooms with JWT-based authentication.

---

## 🚀 Tech Stack

### 🔹 Backend
- Java 17
- Spring Boot
- Spring MVC
- Spring Data JPA (Hibernate)
- Spring Security
- JWT Authentication
- MySQL
- Swagger (API Documentation)

### 🔹 Frontend
- React.js
- Axios
- React Router
- Bootstrap / Tailwind CSS

### 🔹 Tools & DevOps
- Maven
- Git & GitHub
- Postman (API Testing)
- Docker (Optional)

---

## 🏗️ Architecture

This project follows a **3-Tier Architecture**:

Frontend (React)  
        ↓  
Backend (Spring Boot REST APIs)  
        ↓  
Database (MySQL)
![WhatsApp Image 2026-02-26 at 10 56 08](https://github.com/user-attachments/assets/51127688-df88-4fc5-8e0b-2e2e0486b3bf)


### Layers

1️⃣ Presentation Layer – React UI  
2️⃣ Business Logic Layer – Spring Boot Services  
3️⃣ Data Access Layer – JPA Repositories + MySQL  

---

## 🔐 Authentication & Security

- JWT-based Authentication
- Role-Based Access Control (USER / ADMIN)
- Password Encryption (BCrypt)
- Secure REST APIs
- Input Validation
- Rate Limiting

### JWT Flow

1. User logs in  
2. Backend generates JWT token  
3. Token stored on frontend  
4. Token sent in Authorization header  
5. Backend validates token before processing request  

---

## 🛏️ Booking Workflow

1. Search hotels by location, date, price  
2. Filter rooms by category & amenities  
3. Check availability  
4. Apply promo code (optional)  
5. Confirm booking  
6. Update room availability  
7. Generate reservation number  
8. Send email confirmation  

---

## ✨ Core Features

✔ Browse hotels & rooms  
✔ Advanced search & filters  
✔ Secure booking process  
✔ Real-time availability updates  
✔ Booking history for users  
✔ Promotions & discount codes  
✔ Email confirmation system  
✔ Admin management portal  

---

## 📡 REST API Endpoints

### Authentication
- POST `/api/auth/register`
- POST `/api/auth/login`

### Hotels
- GET `/api/hotels`
- GET `/api/hotels/{id}`
- POST `/api/hotels` (Admin)

### Rooms
- GET `/api/rooms`
- GET `/api/rooms/search`

### Bookings
- POST `/api/bookings`
- GET `/api/bookings/user`
- DELETE `/api/bookings/{id}`

### Promotions
- POST `/api/promotions`
- GET `/api/promotions`

---

## 🗄️ Database Design

Main Entities:

- User
- Hotel
- Room
- Booking
- Promotion

Relationships:

- One Hotel → Many Rooms  
- One User → Many Bookings  
- One Room → Many Bookings  

---

## 📂 Project Structure

### Backend
controller
- service
- repository
- model
- dto
- security
- config
- exception

### Frontend
src/
- components
- pages
- services
- context
- utils
- App.js


---

## 🧪 API Documentation

Swagger UI available at:

http://localhost:8080/swagger-ui/

All endpoints tested using Postman.

---

## 🛠️ Installation & Setup

### Backend

```bash
git clone https://github.com/dheerajha/hotel-booking-system.git
cd backend
mvn clean install
mvn spring-boot:run
```

### Frontend

```bash
cd frontend
npm install
npm start
```

