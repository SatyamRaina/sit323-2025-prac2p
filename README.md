This repository contains a basic Node.js application created with the Express.js framework. This application serves a basic HTTP request and response, exhibiting fundamental knowledge of web application development.

📚 Overview

This practical demonstrates the setup of a Node.js server that returns a simple welcome message ("Welcome! STAN") when accessing the root URL of the web server.

✅ Objective

--> Set up a basic Express server.
--> Handle HTTP GET requests.
--> Send a textual response to the client.

📁 Repository Structure

sit323-2025-prac2p/
├── node_modules/
├── package.json
├── package-lock.json
├── server.js
└── README.md

🚀 Technologies Used

Node.js – JavaScript runtime environment.
Express.js – Web application framework for Node.js.

⚙️ Step-by-Step Guide (How This Project Was Created)

Follow these instructions to replicate this project:

Step 1: 
Initialize the Project Folder
Open your terminal and run:
  mkdir sit323-2025-prac2p
  cd sit323-2025-prac2p
  
Step 2: 
Initialize Node Project & Install Dependencies
Run these commands to set up your package.json file and install Express:

  npm init -y
  npm install express
  
Step 3: 
Create the Express Server (server.js)
Create a file called server.js and add the following code:

  const express = require('express');
  const app = express();
  const port = 3000;

  app.get('/', (req, res) => {
    res.send('Welcome! STAN');
  });

  app.listen(port, () => {
    console.log(`Example app listening at http://localhost:${port}`);
  });
  
Step 4: 
Run the Server Locally
Run this command in your terminal:

  node server.js
  
You should see:

  Example app listening at http://localhost:3000
  
Step 5: 
Verify the Application
Open your browser and navigate to: http://localhost:3000

The page should display:

Welcome! STAN
