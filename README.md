# Blog Web Application 

A simple blog web application that allows users to view, create, edit, and delete blog posts. The application is built using Node.js, Express, and EJS for rendering the frontend. The API for handling blog posts operates independently of the frontend server and provides routes for CRUD operations (Create, Read, Update, and Delete).

## Features
• View all blog posts on the main page.  
• Create new blog posts.  
• Edit existing blog posts.  
• Delete blog posts.  
• Simple in-memory storage for blog posts in the API (no database required).

## Technologies Used
• Backend: Node.js, Express  
• Frontend: EJS (Embedded JavaScript Templates)  
• HTTP Client: Axios  
• Middleware: Body-parser for handling request bodies.  
 ## Project Structure  
• server.js: Handles the frontend server that interacts with the API for rendering pages.  
• index.js: Provides the API for managing blog posts (retrieving, creating, editing, and deleting).

## Setup Instructions
### Prerequisites
Ensure you have the following installed:

• Node.js (v12 or higher)  
• npm (comes with Node.js)  


## Clone the Repository
git clone https://github.com/sandygeorge0703/blog-web-application.git  
cd blog-web-application

## Install Dependencies
Install the necessary dependencies by running:

npm install

## Running the Application
The application is split into two parts: the API server and the frontend server. Follow the steps below to run both servers.

### 1. Start the API Server (index.js)  
This server runs on port 4000 and handles the blog post data.

node index.js

You should see:

API is running at http://localhost:4000

### 2. Start the Frontend Server (server.js)
This server runs on port 3000 and serves the front-end pages (using EJS) by communicating with the API.

node server.js

You should see:

Backend server is running on http://localhost:3000

## Viewing the Application
• Navigate to http://localhost:3000 to view the blog application.  
• You can create new posts, edit existing posts, and delete posts through the UI.

### API Endpoints
The API server (index.js) provides the following endpoints for managing blog posts:

• GET /posts: Retrieve all posts.  
• GET /posts/
: Retrieve a specific post by ID.  
• POST /posts: Create a new post.  
• PATCH /posts/
: Update an existing post by ID.  
• DELETE /posts/
: Delete a post by ID.
