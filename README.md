# Hotel Booking Management System

A comprehensive hotel booking and management application built with **Spring Boot** and **Angular**. This system streamlines hotel operations, including guest registration, room administration, and reservation tracking.

## 🚀 Features

- **Guest Management**: Comprehensive profiles for guests and user account management.
- **Room Administration**: Dynamic control over room types, pricing, and availability.
- **Advanced Booking**: Seamless creation, modification, and cancellation of reservations.
- **Real-time Availability**: Instant tracking of room status.
- **Secure Authentication**: Robust security using Spring Security and JWT.
- **Payment Integration**: Supports both **Stripe** and **PayPal** for secure transactions.
- **Mail Services**: Automated notifications for booking confirmations.
- **API Documentation**: Integrated **Swagger/OpenAPI** for easy API exploration.

---

## 🛠️ Tech Stack

### Backend
- **Framework**: Spring Boot 3.4.12
- **Language**: Java 17
- **Database**: MySQL (with Spring Data JPA / Hibernate)
- **Security**: Spring Security & JWT
- **APIs**: RESTful Services with SpringDoc OpenAPI (Swagger)
- **Payments**: Stripe Java SDK & PayPal Checkout SDK
- **Utilities**: Lombok, ModelMapper, Spring Dotenv

### Frontend
- **Framework**: Angular (Next Gen)
- **Language**: TypeScript
- **Payments**: ngx-stripe & @stripe/stripe-js
- **Testing**: Vitest & JSDOM
- **Styling**: Vanilla CSS

---

## 📂 Project Structure

```text
hotel_Booking_Management/
├── angular_frontend/    # Angular Frontend Application
├── spring_backend/      # Spring Boot Backend API
└── README.md             # Project documentation
```

---

## ⚙️ Getting Started

### Prerequisites
- **Java JDK 17**
- **Node.js** (v18 or higher)
- **MySQL Server**
- **Maven** (optional, wrapper included)

### 1. Database Setup
Create a MySQL database named `hotel`:
```sql
CREATE DATABASE hotel;
```

### 2. Backend Configuration
Navigate to `spring_backend/src/main/resources/application.properties` or create a `.env` file in the `spring_backend` root with the following:
```env
DB_USERNAME=your_mysql_user
DB_PASSWORD=your_mysql_password
JWT_KEY=your_secret_jwt_key
MAIL_USERNAME=your_gmail
MAIL_PASSWORD=your_gmail_app_password
STRIPE_PUBLIC_KEY=your_stripe_public_key
STRIPE_SECRET_KEY=your_stripe_secret_key
PAYPAL_CLIENT_ID=your_paypal_client_id
PAYPAL_SECRET_KEY=your_paypal_secret_key
```

### 3. Run the Backend
```bash
cd spring_backend
./mvnw spring-boot:run
```
The API will be available at `http://localhost:8080`.
You can access the API documentation at `http://localhost:8080/api-docs`.

### 4. Run the Frontend
```bash
cd angular_frontend
npm install
npm start
```
The application will be accessible at `http://localhost:4200`.

---

## 🧪 Testing
- **Backend**: Run `./mvnw test`
- **Frontend**: Run `npm test`

## 📝 License
This project is licensed under the [MIT License](LICENSE).

## 👨‍💻 Author
**Phan Thiết Trung**

---
*Last updated: March 2026*

