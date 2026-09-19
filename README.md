# 🍔 FoodXpress — Online Food Delivery Platform

FoodXpress is a modern, full-stack Java EE web application for online food ordering, restaurant discovery, order tracking, and customer reviews.

---

## 📌 Module Overview — Part 3: Customer Portal & Web Interface

This repository contains **Part 3: Customer Portal & Web Interface**, which handles the complete end-to-end customer journey from user authentication, browsing menus, adding items to cart, placing orders, and submitting restaurant ratings & reviews.

### 👥 Team Contribution
* **Module**: Part 3 — Customer Portal & Web Interface
* **Contributor**: Tashin Mustakim (`tashinmustakim`)

---

## ✨ Features Implemented in Customer Portal

* 🔐 **User Authentication & Session Management**:
  * User Registration & Login with encrypted passwords and session tracking.
  * Profile management and personal order history.
* 🍴 **Restaurant & Menu Browsing**:
  * Browse active restaurants with cuisine filters, addresses, and live ratings.
  * Interactive restaurant menu view with item descriptions and prices.
* 🛒 **Shopping Cart & Checkout**:
  * Dynamic cart session management (add, update quantity, remove items).
  * Subtotal, tax, delivery fee, and grand total calculations.
  * Checkout workflow with address input and order summary.
* 📜 **Order History & Delivery Tracking**:
  * Detailed past order listing with status badges (`PENDING`, `PREPARING`, `OUT_FOR_DELIVERY`, `DELIVERED`, `CANCELLED`).
  * Invoice and item breakdown per order.
* ⭐ **Customer Reviews & Rating System**:
  * Submit star ratings (1–5 Stars) and feedback comments for restaurants.
  * Live restaurant average rating recalculation.

---

## 🛠️ Technology Stack

* **Backend**: Java EE (Servlets & JSTL 1.2), Maven
* **Frontend**: JSP (JavaServer Pages), Vanilla CSS3 (Custom Design System with Glassmorphism & Modern Micro-animations), HTML5
* **Database**: MySQL 8.0 JDBC Connector (`food_delivery_app` schema)
* **Application Server**: Apache Tomcat / Eclipse Jetty 10

---

## 📂 Project Structure (Part 3)

```text
part3_customer_portal/
├── README.md
└── src/
    └── main/
        ├── java/
        │   └── com/
        │       └── app/
        │           └── controllers/
        │               ├── HomeServlet.java
        │               ├── UserServlet.java
        │               ├── RestaurantServlet.java
        │               ├── MenuServlet.java
        │               ├── CartServlet.java
        │               ├── CheckoutServlet.java
        │               ├── OrderHistoryServlet.java
        │               └── ReviewServlet.java
        └── webapp/
            └── jsp/
                ├── customer/
                │   ├── home.jsp
                │   ├── login.jsp
                │   ├── register.jsp
                │   ├── restaurantList.jsp
                │   ├── restaurantDetails.jsp
                │   ├── cart.jsp
                │   ├── checkout.jsp
                │   ├── orderHistory.jsp
                │   ├── orderSuccess.jsp
                │   └── profile.jsp
                └── shared/
                    ├── head.jspf
                    ├── header.jspf
                    └── footer.jspf
```

---

## 🚀 How to Run Locally

1. Ensure MySQL server is running with the `food_delivery_app` schema.
2. Clone the core models (`Part 1`) and DAOs (`Part 2`) into your classpath/project.
3. Build the project using Maven:
   ```bash
   mvn clean compile jetty:run
   ```
4. Access the application in your web browser:
   ```text
   http://localhost:8085/FoodApp/
   ```

---

## 📜 License
This project is open source and available for academic and educational evaluation.
