# Multivendor E-commerce Platform

This project is a full-stack multivendor e-commerce platform that allows multiple vendors to register and manage their own stores. Customers can browse, purchase products, and leave reviews. Admins have full control over managing vendors, products, orders, and other operations. The project uses Spring Boot for the backend and Angular for the frontend.

## Features

### Admin Panel
- Manage vendors, products, orders, and customers.
- Control shipping rates based on location and product weight.
- Oversee financial transactions and shipping logistics.
- Admin access to reports and analytics.

### Vendor Panel
- Manage inventory, products, and stock.
- Track orders, customer reviews, and analytics.
- Update product details, images, and descriptions.
- Monitor shipping status and order fulfillment.

### Customer Panel
- Register, log in, and manage profiles.
- Browse products by category and brand.
- Add products to the cart, place orders, and track shipping.
- Leave product reviews and rate the quality.
- Ask and answer product-related questions.

### Core Features
- **Role-based access control**: Different permissions for Admins, Vendors, and Customers using Spring Security.
- **Email verification**: Account registration with email confirmation.
- **RESTful API**: Communicates between the backend (Spring Boot) and frontend (Angular).
- **Online payment**: Integrated PayPal Sandbox for secure payment transactions.
- **Shipping calculation**: Dynamic calculation of shipping fees based on location and product weight.

## Database Structure

The database is structured into several modules, including products, orders, customers, vendors, and shipping rates. Below is an overview of the main tables and their relationships.

### Database Overview

### Customer Module
- `customers`: Stores customer information, including their contact details, addresses, and account status.
- `addresses`: Stores customer addresses for shipping and billing purposes.
- `reviews`: Contains customer reviews and ratings for products.
- `cart_items`: Stores the items in a customer's shopping cart.

### Product Module
- `products`: Stores product details, such as price, description, dimensions, and stock status.
- `categories`: Stores product categories and their hierarchical relationships.
- `order_details`: Tracks information about each product in a customer's order.

### User Module
- `users`: Contains basic user information, including their role (Admin, Vendor, Customer).
- `roles`: Defines user roles and permissions.
- `users_roles`: Associates users with their respective roles in the system.


