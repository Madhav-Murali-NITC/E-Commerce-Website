E-Commerce Platform Documentation
Problem Statement
In the rapidly evolving landscape of online commerce, businesses face the challenge of providing a seamless and engaging shopping experience for users while ensuring efficient management of products and orders. Furthermore, maintaining data integrity, scalability, and security poses significant challenges in the development of e-commerce platforms.

Solution Overview
To address these challenges, we have developed a comprehensive e-commerce platform leveraging modern web technologies and robust database design principles. Our solution focuses on delivering a user-friendly interface, efficient data management, and stringent security measures.

Architecture Overview
Our platform is built upon a foundation of industry-standard technologies, prominently featuring React for the frontend, Express and Node.js for the backend, MySQL for database management, and standard web technologies (HTML, CSS, JavaScript) for user interface design and interactivity.

Database Design
Central to the efficacy of our platform is the database architecture, meticulously structured according to the principles of the third normal form (3NF). This design paradigm ensures optimal data organization, minimizes redundancy, and enhances scalability. By adhering to 3NF, our database system maintains data integrity, facilitates efficient querying, and lays a robust foundation for future expansion.

Backend Implementation
The backend functionality is orchestrated through Express.js, a minimalist web application framework for Node.js. Leveraging Express, we have implemented a suite of RESTful APIs to facilitate seamless communication between the frontend and backend components. These APIs handle critical functionalities such as user authentication, product management, and cart operations.

Frontend Development
The frontend interface, designed with user-centricity in mind, is crafted using React – a declarative and component-based JavaScript library. Through React, we have engineered an intuitive and visually appealing user interface, fostering a delightful browsing and shopping experience for our users. HTML and CSS are employed extensively to structure and style the various components, ensuring accessibility and responsiveness across devices.

Key Features
Our e-commerce platform boasts several key features designed to enhance user engagement and administrative efficiency:

Cart System: A robust cart management system enabling users to add, remove, and modify items in their shopping carts seamlessly.
Product Management: Comprehensive tools for administrators to effortlessly add, update, and remove products from the platform, ensuring a dynamic and up-to-date catalog.
Role-based Authentication: A sophisticated authentication mechanism that distinguishes between user roles (e.g., regular user, admin), ensuring secure access control and privilege management.
Backend Routes Overview
Authentication Routes (auth.js):

Login Route (/auth/login): Validates email and password fields, checks user existence, compares passwords, and generates JWT tokens upon successful authentication.
Registration Route (/auth/register): Validates email and password fields, checks for existing email/username, hashes passwords, and inserts users into the database.
Cart Routes (cart.js):

Get Cart Items Route (/cart/:id): Retrieves cart items for a specific user from the database.
Add to Cart Route (/cart/new/:id): Adds a new product to the user's cart in the database.
Order Routes (orders.js):

Get User Orders Route (/orders/:id): Retrieves order history for a specific user from the database.
Get Order Details Route (/orders/order/:id): Retrieves details of a specific order by its ID.
Place New Order Route (/orders/new/:id): Inserts a new order into the database for a specific user.
Product Routes (products.js):

Get All Products Route (/products): Retrieves all products from the database with pagination support.
Get Products by Category Route (/products/:catName): Retrieves products belonging to a specific category with pagination support.
Get Product by Name Route (/products/name/:name): Retrieves product details based on the provided name.
Admin Routes (/products/admin): Provides CRUD operations for products with admin privileges.
Database Connection
Establishes a MySQL database connection using the mysql package.
Handles errors during the connection process.
Automatically closes the connection when the application exits.
Overall Design
The backend follows a modular design, with each route grouped into separate files (auth.js, cart.js, orders.js, products.js).
Utilizes Express.js to create and manage routes.
Implements JWT-based authentication for user sessions.
Uses bcrypt for password hashing and validation.
Employs MySQL queries to interact with the database.
Provides RESTful endpoints for user authentication, cart management, order processing, and product management.
This backend system facilitates user authentication, cart management, order processing, and product management functionalities for an e-commerce platform.

Frontend Implementation
TBD
