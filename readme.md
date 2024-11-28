# Authentication and Authorisation system 
It uses EJS Templates,Node.js, Express, and MongoDB to manage the backend and database. 
The project includes a combined API for seamless integration of functionalities.


### Idea


### Features
1. User Authentication: Secure login and signup functionality using JWT.
2. Role-Based Authorization: APIs accessible based on user roles.
3. Session Timeout: Automatic logout after 15 minutes of inactivity.
4. Secure Password Handling: Passwords are hashed with bcrypt.
5. Dynamic Views: Built with EJS templates for a clean user interface.

Includes sample MongoDB data for quick setup and testing.

### Tech Stack
Backend: Node.js, Express.js
Database: MongoDB
Authentication: JWT (JSON Web Tokens)
Frontend: EJS templates
Session Management: JWT with session expiration
Password Security: bcrypt.js
Tools: MongoDB Database Tools (mongodump)

### Setup Instructions

#### Prerequisites
1.  Install Node.js  https://nodejs.org/en/download/package-manager
2.  Install MongoDB Compass or use MongoDB Atlas (Cloud MongoDB).
3.  Install MongoDB Database Tools for mongodump and mongorestore if needed:
        Download MongoDB Tools.

#### Installation
1.  Clone the Repository:  
    ##
        git clone https://github.com/Akanksha1301/assignment2024.git
        cd assignment2024

2.  Install Dependencies
    ##
        npm install express mongoose dotenv bcryptjs jsonwebtoken express-session connect-mongo cookie-parser ejs
        npm install --save-dev nodemon

#### Import sample data
1.  Start MonoDB
    ##
        mongo

2.  Restore the dump
    ##
        mongorestore --db ecommerce dump/ecommerce

3.  Verify Data
    ##
        mongo
        use ecommerce
        db.warehouse.find().pretty()
        db.customer.find().pretty()

#### Run the Application
1.  Start the development server
    ##
        nodemon start
The server will run on http://localhost:5000.

### Start the app using URL

1. Login Page
Path: views/login.ejs

This page allows users to log in.

2. Signup Page
Path: views/signup.ejs

This page allows new users to sign up.

3. Dashboard
Path: views/dashboard.ejs

Displays user-specific data.


### How to Run Locally
Ensure MongoDB is running locally.
Install dependencies with npm install.
Start the server with npm start.
Access the app at http://localhost:5000.


### Testing the APIs
   Use Postman or Curl to test the APIs.

