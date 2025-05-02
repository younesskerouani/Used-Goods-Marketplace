
# JotiaShop - E-Commerce Platform for Used Products
![z1](https://github.com/user-attachments/assets/0b2dec4d-9020-4897-8b5d-f72361efd8b8)


## 📋 Overview

JotiaShop is a comprehensive e-commerce platform specifically designed for the sale of used products. platform offers a sustainable alternative to buying new, giving pre-owned products a second life while providing value to both sellers and buyers.

## 📸 Screenshots

### Product Categories
![z2](https://github.com/user-attachments/assets/2dcc527e-5f04-40de-b92a-39ce22a96291)


### Product Detail Page
![z3](https://github.com/user-attachments/assets/1265000e-c8b1-4f68-8ddb-9e457ba2068c)
![z4](https://github.com/user-attachments/assets/156c6bf7-395c-4696-99ac-9f1106aca562)


### Shopping Cart
![z5](https://github.com/user-attachments/assets/2ee96315-70c7-4b21-ad3f-23dfda7467a2)


## 💳 Payment Methods

JotiaShop offers secure payment processing through:
- **PayPal**: Our primary payment gateway, allowing customers to pay with their PayPal account or credit card
- **Credit/Debit Card**: Direct payment option via secure processing

## ✨ Features

### 🛒 Front-end Features
- **Product Browsing**: Search by name or browse by category (Electronics, Casual Shirts, Sneakers, etc.)
- **User Accounts**: Register and sign in to access personalized features
- **Shopping Cart**: Add products, view your bag, and process orders
- **Product Pages**: Detailed product information with structured data including:
  - Product name
  - Product rating
  - Product photos
  - Detailed description
  - Region of origin
  - Seller information
- **User Reviews**: Post comments and reviews on products
- **Secure Checkout**: Multiple payment options including PayPal and credit card

### ⚙️ Back-office Features
- **Seller Dashboard**: Complete management interface for vendors
- **Inventory Management**: Add, modify, or remove products
- **Order Tracking**: Monitor order status (processing, shipping, delivered)
- **Stock Management**: Track inventory levels for each product
- **Sales Analytics**: Monitor performance and sales data

## 🔧 Technical Information

### Built With
- Frontend: React.js
- Backend: Java Spring Boot
- Database: MySQL
- Payment Processing: PayPal integration (primary payment method)

### Key Features Implementation
- **Product Management**: Full CRUD operations for sellers
- **User Authentication**: Secure login and registration system
- **Shopping Cart**: Real-time cart management
- **Order Processing**: End-to-end order management
- **PayPal Integration**: Secure payment processing
- **Responsive Design**: Mobile-friendly interface

## 🚀 Getting Started

### Prerequisites
```
- Java 8 (JDK 1.8)
- Spring Boot 2.4.2
- Node.js 14.x or higher
- npm 6.x or higher
- MySQL 5.1.x
- Maven 3.6.x or higher
- Lombok
```

### Setup Instructions
**1. Clone the repository**
```
  bash

  git clone https://github.com/yourusername/jotiashop.git
  cd jotiashop
```
**2. Database Setup**
```
bash

mysql -u your_username -p < db4.sql

```
This creates all necessary tables: categorie, product, users, and hibernate_sequence.

**3. Backend Configuration**
``` 
cd backend
```
Edit src/main/resources/application.properties:

```

spring.datasource.url=jdbc:mysql://localhost:3306/db4?useSSL=false 
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL5Dialect
spring.jpa.show-sql=true
```
Build and run:

```
mvn clean install
mvn spring-boot:run
```
Backend server will start at http://localhost:8080

**4. Frontend Configuration**
This creates all necessary tables: categorie, product, users, and hibernate_sequence.

```
cd ../front
npm install
```
Create .env file:
```
REACT_APP_API_URL=http://localhost:8080/api
REACT_APP_PAYPAL_CLIENT_ID=your_paypal_client_id
```

Start the frontend:
```
npm start
```
Frontend will be available at http://localhost:3000


**📖 Usage**

*For Customers*

Browse products by category or use the search function
Create an account to save favorites and process orders
Add products to your shopping cart
Complete checkout using your preferred payment method

*For Sellers*

Create a seller account with your email and password
Access your seller dashboard
Add products with detailed descriptions and photos
Monitor orders and manage your inventory

