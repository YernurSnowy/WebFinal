# Yernur Koishybayev 

# Laptops Hub 🖥️

This is a web application named "Laptops Hub," built with Node.js and Express.js, designed to provide various functionalities related to technology products and services.

## Features

- **User Registration and Authentication:** The application allows users to create accounts with unique usernames and passwords, ensuring secure authentication through bcrypt for password hashing.
- **Session Management:** Utilizing express-session, the system efficiently manages user sessions to maintain login status across requests.
- **Phone Management:** Users can perform CRUD (Create, Read, Update, Delete) operations on phones, including adding, editing, and deleting phone records.
- **Admin Panel:** Administrators are provided access to an admin panel, empowering them to oversee and manage all phone entries within the system.
- **MongoDB Integration:** Data storage and management are seamlessly handled with MongoDB, leveraging Mongoose as the ODM library for Node.js to streamline object modeling.
- **Email Notification:** Upon successful registration, users receive a welcome email, facilitated by Nodemailer for sending emails via SMTP, enhancing user engagement and communication.
- **Static File Serving:** Express.js serves static files such as CSS and JavaScript, enriching the user interface with enhanced styling and interactivity.

## Installation

1. Download a ZIP file
2. Install dependencies:

    ```bash
    npm install
    ```

3. Set up environment variables:

   Create a `.env` file in the root directory and add the following variables:

    ```env
    PORT=3000
    MONGODB_URL="YOUR URL TO MONGODB"
    EMAIL_USER="YOUR EMAIL"
    EMAIL_PASS="YOUR PASSWORD TO EAMIL"
    ```

4. Start the project:

   `npm run start`

5. Access the application:

   Open your web browser and visit `http://localhost:3000`.

## Usage

- Visit `http://localhost:3000/register` to register for a new account.
- After registration, login at `http://localhost:3000/login`.
- Add, edit, or delete items in the portfolio at `http://localhost:3000/dashboard`.
- Administrators can access the admin panel at `http://localhost:3000/admin` to manage all items.

## Dependencies

- Express.js 🚀: Web application framework for Node.js
- Mongoose 🏬: MongoDB object modeling for Node.js
- bcrypt 🔒: Library for password hashing and salting
- express-session 🕸️: Session middleware for Express.js
- Nodemailer 📧: Library for sending emails from Node.js
- dotenv 🛠️: Loads environment variables from a .env file into process.env


Sure, here's how you can explain the three APIs used in the provided code in the README:

---

# API'S

The application utilizes three external APIs to enrich its features:

## 1. IP Geolocation API
The IP Geolocation API is employed to ascertain the geographical location of the user based on their IP address. By capturing the user's IP address, the application queries the IP Geolocation API to retrieve details such as country, city, and coordinates. This information enhances user experience by offering location-specific content and services.

API Endpoint: https://ipapi.co/json/ 🌍

##2. FonoAPI
The FonoAPI serves as a comprehensive database of device specifications, including smartphones, tablets, and other electronic gadgets. In the application, this API is utilized to fetch detailed specifications of various tech products. Users can access this information to compare devices, view specifications, and make informed purchasing decisions.

API Endpoint: https://fonoapi.freshpixl.com/v1/📱

##3. ExchangeRate API
The ExchangeRate API provides real-time and historical foreign exchange rates. In the context of the "Apple Tech Hub" application, this API is integrated to facilitate currency conversion for international users. By accessing current exchange rates, the application enables users to view prices in their preferred currency, promoting a seamless shopping experience across different regions.

API Endpoint: https://api.exchangerate-api.com/💱

---
