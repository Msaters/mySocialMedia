# MySocialMedia 

A social media application built using the **MERN** stack (MongoDB, Express, React, Node.js). This project serves as a testing playground to learn full-stack development, focusing on building a highly secure authentication system.

## Project Status

**Work unfinished** The core authentication and user management module is fully completed. Other social media features (like posting or commenting) are unfinished.

## Key Features

* **User Registration:** Users can create new accounts, and initial profile data is assigned to them in the database.
* **Password Encryption:** Passwords are not stored in plain text. They are securely hashed/encrypted before saving them to MongoDB to ensure data safety.
* **Dual-Token Authentication System:** Adheres to modern security best practices:
  * **Access Token:** A short-lived token (valid for a few minutes) used for secure API requests.
  * **Refresh Token:** A long-lived token (valid for months) used to seamlessly request a new Access Token behind the scenes when the old one expires.

## Tech Stack

* **Frontend:** React.js, HTML, CSS
* **Backend:** Node.js, Express.js
* **Database:** MongoDB
* **Testing:** Postman (API)

## How to Run

Since the project is divided into a frontend and a backend, you will need to start both servers separately. Make sure you have [Node.js](https://nodejs.org/) installed.

**1. Start the Backend (API):**
Open a terminal, navigate to the `backend` folder, install the dependencies, and start the server using `nodemon` (which automatically restarts the server when you make code changes):
```bash
cd backend
npm install
nodemon index.js
```

**Start the Frontend (User Interface):**
Open a new terminal window, navigate to the frontend folder, install dependencies, and start the React app:
```bash
cd frontend
npm install
npm start
```

The application will automatically open in your web browser at http://localhost:3000.
