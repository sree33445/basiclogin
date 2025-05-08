# HTML Login Signup Backend

This is the backend for a login and signup system built using Node.js, Express, and PostgreSQL.

## Features

- User registration with hashed passwords
- User login with JWT authentication
- PostgreSQL database integration

## Prerequisites

Before running this project, ensure you have the following installed:

- [Node.js](https://nodejs.org/)
- [PostgreSQL](https://www.postgresql.org/)
- [npm](https://www.npmjs.com/)

## Installation

1. Clone the repository:
   
   git clone <repository-url>
   cd htmlloginsignup/backend
   npm install

2.Create a .env file in the root directory and add the following environment variables:
    
    DB_HOST=<your-database-host>
    DB_PORT=<your-database-port>
    DB_USER=<your-database-username>
    DB_PASSWORD=<your-database-password>
    DB_NAME=<your-database-name>
    JWT_SECRET=<your-jwt-secret>

3.Set up the PostgreSQL database:

   Create a database.
   Create a users table:

    CREATE TABLE users (
    id SERIAL PRIMARY KEY,
    name VARCHAR(255) NOT NULL,
    email VARCHAR(255) UNIQUE NOT NULL,
    password VARCHAR(255) NOT NULL
    );
4.Run the server using:
 node server.js
