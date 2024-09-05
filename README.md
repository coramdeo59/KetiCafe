Introduction

KetiCafe is a full-stack web application designed to manage the operations of a cafe. This project includes features for managing menu items, handling customer orders, and processing reservations. Built with a modern tech stack, KetiCafe aims to streamline the day-to-day operations of a cafe while providing customers with a seamless online experience.

Whether you're looking to manage your cafe's menu, allow customers to make reservations, or offer online ordering, KetiCafe provides the tools to make it happen.
Project Structure

The project is structured as a monorepo containing both the frontend and backend components.

KetiCafe/
│
├── client/                  # Frontend (React)
│   ├── public/
│   ├── src/
│   ├── package.json
│   ├── .env
│   └── ...
│
├── server/                  # Backend (Express)
│   ├── config/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── server.js
│   ├── .env
│   └── ...
│
└── ...
Features
User-Facing Features

    Menu Browsing: Customers can browse the cafe's menu items, including descriptions, prices, and images.
    Online Ordering: Customers can place orders online and get real-time updates on their order status.
    Reservations: Users can book tables in advance, specifying the number of guests and the time of the reservation.
    Customer Reviews: Allows customers to leave reviews and ratings for their experience.

Admin Features

    Menu Management: Admins can add, edit, or remove menu items through a simple interface.
    Order Management: Admins can track and update order statuses (e.g., pending, in progress, completed).
    Reservation Management: Manage and confirm reservations from customers.
    User Management: Admins can manage users, including roles and permissions.

Technology Stack
Frontend

    React: The main framework for building the user interface.
    React Router: For handling page navigation.
    Axios: For making HTTP requests to the backend API.
    Bootstrap or TailwindCSS: (Depending on your choice) For styling and responsive design.

Backend

    Node.js: The runtime environment.
    Express.js: The web framework for building the RESTful API.
    MongoDB: The NoSQL database for storing application data.
    Mongoose: For modeling and interacting with MongoDB.
    JWT: For authentication and authorization.

DevOps & Tools

    Docker: Containerization for easy deployment.
    Docker Compose: To manage multi-container Docker applications.
    Nginx: As a reverse proxy (optional).
    GitHub Actions: For CI/CD pipeline (optional).
    Postman: For API testing and documentation.

Setup and Installation
Prerequisites

Before you begin, ensure you have the following installed:

    Node.js (v14+)
    npm or Yarn
    MongoDB (locally or using a cloud service like MongoDB Atlas)
Clone the Repository

bash

git clone https://github.com/coramdeo59/KetiCafe.git
cd KetiCafe

Environment Variables

Create a .env file in both the client/ and server/ directories. Example:
For the Client

bash

REACT_APP_API_URL=http://localhost:5000/api

For the Server

bash

PORT=5000
MONGO_URI=mongodb://localhost:27017/keticafe
JWT_SECRET=your_jwt_secret

Install Dependencies
For the Client

bash

cd client
npm install

For the Server

bash

cd server
npm install

Running the Application
Running Locally

    Start the Backend Server:

    bash

cd server
npm start

This will start the Express server on http://localhost:5000.

Start the Frontend:

In another terminal window, navigate to the client/ directory and run:

bash

    npm start

    The React app will run on http://localhost:3000.

Running with Docker

You can run the entire application using Docker. Ensure Docker is installed and running on your machine.

    Build and Start Containers:

    bash

docker-compose up --build

This will start both the frontend and backend services.

Access the Application:

    Frontend: http://localhost:3000
    Backend: http://localhost:5000
