# E-Commerce Platform Documentation

## Problem Statement
In the rapidly evolving landscape of online commerce, businesses face the challenge of providing a seamless and engaging shopping experience for users while ensuring efficient management of products and orders. Furthermore, maintaining data integrity, scalability, and security poses significant challenges in the development of e-commerce platforms.

## Solution Overview
To address these challenges, we have developed a comprehensive e-commerce platform leveraging modern web technologies and robust database design principles. Our solution focuses on delivering a user-friendly interface, efficient data management, and stringent security measures.

## Architecture Overview
Our project primarily uses React for the frontend, Express and Node.js for the backend, MySQL for database management, and standard web technologies (HTML, CSS, JavaScript) for user interface design and interactivity.

## Database Design
![FLOWCHART](https://github.com/Madhav-Murali-NITC/E-Commerce-Website/blob/main/er-ecommerce.jpeg)


## Key Features
Our e-commerce platform boasts several key features designed to enhance user engagement and administrative efficiency:
- **Cart System**: A robust cart management system enabling users to add, remove, and modify items in their shopping carts seamlessly.
- **Product Management**: Comprehensive tools for administrators to effortlessly add, update, and remove products from the platform, ensuring a dynamic and up-to-date catalog.
- **Role-based Authentication**: A sophisticated authentication mechanism that distinguishes between user roles (e.g., regular user, admin), ensuring secure access control and privilege management.
- **Order Management System**: A personalized platform enabling individual users to seamlessly checkout items within their cart, while offering diverse payment methods for a tailored experience.

## Backend Routes Overview
- **Authentication Routes (auth.js):**
  - *Login Route (/auth/login)*: Validates email and password fields, checks user existence, compares passwords, and generates JWT tokens upon successful authentication.
  - *Registration Route (/auth/register)*: Validates email and password fields, checks for existing email/username, hashes passwords, and inserts users into the database.
- **Cart Routes (cart.js):**
  - *Get Cart Items Route (/cart/:id)*: Retrieves cart items for a specific user from the database.
  - *Add to Cart Route (/cart/new/:id)*: Adds a new product to the user's cart in the database.
- **Order Routes (orders.js):**
  - *Get User Orders Route (/orders/:id)*: Retrieves order history for a specific user from the database.
  - *Get Order Details Route (/orders/order/:id)*: Retrieves details of a specific order by its ID.
  - *Place New Order Route (/orders/new/:id)*: Inserts a new order into the database for a specific user.
- **Product Routes (products.js):**
  - *Get All Products Route (/products)*: Retrieves all products from the database with pagination support.
  - *Get Products by Category Route (/products/:catName)*: Retrieves products belonging to a specific category with pagination support.
  - *Get Product by Name Route (/products/name/:name)*: Retrieves product details based on the provided name.
  - *Admin Routes (/products/admin)*: Provides CRUD operations for products with admin privileges.


## Overall Design
- The backend follows a modular design, with each route grouped into separate files (auth.js, cart.js, orders.js, products.js).
- Utilizes Express.js to create and manage routes.
- Implements JWT-based authentication for user sessions.
- Uses bcrypt for password hashing and validation.
- Employs MySQL queries to interact with the database.
- Provides RESTful endpoints for user authentication, cart management, order processing, and product management.

