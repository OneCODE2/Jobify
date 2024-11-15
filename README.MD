Jobify - Job Search Tracker

This project helps you track your job search applications. See it in action: Jobify

Support: Found this app useful? Buy me a coffee!

Running the App Locally

Install Dependencies:

npm run install-dependencies
content_copy
Use code with caution.
Bash

Configure Environment Variables:

Rename .env.temp to .env

Set values for MONGO_URL, JWT_SECRET, and JWT_LIFETIME

Start the Server:

npm start
content_copy
Use code with caution.
Bash

Access the App: Visit http://localhost:3000/

Project Setup Overview

This guide outlines the key steps involved in setting up the Jobify application, both the front-end (React) and back-end (Node.js/Express).

Front-End (React):

Create React App:

cd client
npx create-react-app .
npm start
content_copy
Use code with caution.
Bash

Replace Default Files: Copy assets and replace default files (App.js, index.js, etc.) from the complete project into the client folder.

Install Dependencies: Refer to the individual sections below for installing necessary dependencies like normalize.css, styled-components, and react-router-dom.

Implement Pages and Components: Follow the detailed steps in the sections below to build out the various pages (Landing, Register, Dashboard, etc.) and components (Logo, Navbar, etc.).

Back-End (Node.js/Express):

Initialize Node Project:

npm init -y
content_copy
Use code with caution.
Bash

Install Dependencies: Install necessary dependencies like express, mongoose, dotenv, and security packages (see below).

Create Server File: Create server.js and set up the basic Express server.

Connect to Database: Configure the connection to your MongoDB database using Mongoose.

Implement Routes and Controllers: Follow the detailed steps to create controllers and routes for authentication and job management functionality.

Set up Middleware: Implement middleware for error handling, authentication, and security.

Key Project Features and Implementation Details:

Styling: Uses styled-components for CSS-in-JS. normalize.css ensures cross-browser consistency.

Routing: Uses react-router-dom v6 for navigation and nested routes. Protected routes ensure only authenticated users can access certain pages.

State Management: Uses React's useContext and useReducer for managing global application state.

Backend API: Built with Node.js and Express.js.

Database: Uses MongoDB with Mongoose for data persistence.

Authentication: Uses JWT (JSON Web Tokens) for secure authentication. Stores JWT in cookies.

Job Management: Allows users to create, read, update, and delete job applications.

Statistics: Provides visual statistics about job applications using recharts.

Filtering and Sorting: Allows users to filter and sort job applications.

Search: Implements search functionality with optional debouncing.

Security: Uses Helmet, XSS-clean, express-mongo-sanitize, and express-rate-limit for enhanced security.

Test User: Allows users to test the application with a demo account. Read-only access for the test user.

Deployment: Instructions for building and deploying the front-end and back-end.

Detailed Sections (From Original README)

The original README provided granular steps for implementing each feature. If you need more detail on a specific area (e.g., setting up the landing page, implementing the reducer, configuring JWT, etc.), refer back to the original README content provided in your initial prompt. It offers step-by-step guidance and code snippets.

This revised README provides a clearer overview of the project structure and key implementation details. It also emphasizes the essential steps for setting up and running the application locally. Remember to consult the original README for more in-depth instructions on individual components and features.
