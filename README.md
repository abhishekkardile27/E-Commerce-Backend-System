# E-Commerce Backend System

## 📌 Project Overview

E-Commerce Backend System is a REST API based web application developed using Java, Spring Boot, Spring Security, JWT Authentication, Hibernate, JPA, and MySQL.

The application provides secure user authentication and authorization, product management, shopping cart functionality, and order management.

## 🚀 Features

### User Authentication

* User Registration
* User Login
* JWT Token Generation
* Role-Based Authorization
* Secure Password Encryption

### Product Management

* Add Product
* Update Product
* Delete Product
* View All Products
* Search Products

### Cart Management

* Add Product to Cart
* Update Cart Quantity
* Remove Product from Cart
* View Cart Items

### Order Management

* Place Order
* View Order History
* Manage Orders

## 🛠 Technologies Used

### Backend

* Java 17
* Spring Boot
* Spring Security
* Spring Data JPA
* Hibernate
* JWT Authentication

### Database

* MySQL

### Build Tool

* Maven

### API Testing

* Postman

## 📂 Project Structure

src
├── controller
│ ├── AuthController
│ ├── CartController
│ └── OrderController
│
├── service
│ ├── AuthService
│ ├── CartService
│ └── OrderService
│
├── repository
│ ├── UserRepository
│ ├── CartRepository
│ └── OrderRepository
│
├── entity
│ ├── User
│ ├── Product
│ ├── Cart
│ └── Order
│
├── security
│ ├── JwtFilter
│ ├── SecurityConfig
│ └── CustomUserDetailsService

## 🔐 Authentication Flow

1. User registers account.
2. User logs in using email and password.
3. JWT token is generated.
4. Token is sent in Authorization Header.
5. Protected APIs are accessed using JWT token.

Authorization Header:

Bearer <JWT_TOKEN>

## 📡 REST API Endpoints

### Authentication APIs

| Method | Endpoint       | Description   |
| ------ | -------------- | ------------- |
| POST   | /auth/register | Register User |
| POST   | /auth/login    | Login User    |

### Product APIs

| Method | Endpoint       | Description       |
| ------ | -------------- | ----------------- |
| GET    | /products      | Get All Products  |
| GET    | /products/{id} | Get Product By Id |
| POST   | /products      | Add Product       |
| PUT    | /products/{id} | Update Product    |
| DELETE | /products/{id} | Delete Product    |

### Cart APIs

| Method | Endpoint          | Description      |
| ------ | ----------------- | ---------------- |
| POST   | /cart/add         | Add Item To Cart |
| GET    | /cart             | View Cart        |
| DELETE | /cart/remove/{id} | Remove Item      |

### Order APIs

| Method | Endpoint      | Description |
| ------ | ------------- | ----------- |
| POST   | /orders/place | Place Order |
| GET    | /orders       | View Orders |

## ⚙️ Installation & Setup

### Clone Repository

git clone https://github.com/your-username/ecommerce-backend-system.git

### Navigate To Project

cd ecommerce-backend-system

### Configure Database

Update application.properties file:

spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce_db
spring.datasource.username=root
spring.datasource.password=root

### Build Project

mvn clean install

### Run Application

mvn spring-boot:run

Application will start on:

http://localhost:8080

## 🧪 Testing APIs

Use Postman to test APIs.

1. Register User
2. Login User
3. Copy JWT Token
4. Add Token in Authorization Header
5. Access Protected APIs

## Future Enhancements

* Payment Gateway Integration
* Product Image Upload
* Email Notifications
* Admin Dashboard
* Inventory Management

## 👨‍💻 Author

Abhishek

### GitHub

https://github.com/your-github-username

### LinkedIn

https://linkedin.com/in/your-linkedin-profile
