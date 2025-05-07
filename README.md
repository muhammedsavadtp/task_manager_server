Task Manager Backend - Installation and Setup
This is the backend for the Task Manager application, built with Node.js, Express, and MongoDB. It provides a REST API for task management.
Installation and Setup

Prerequisites:

Node.js (v16 or higher)
MongoDB (local or MongoDB Atlas)
npm or yarn


Clone the Repository:
git clone <backend-repository-url>
cd backend


Install Dependencies:
npm install
npm install express mongoose dotenv cors
npm install --save-dev nodemon


Configure Environment Variables:Create a .env file in the backend directory:
echo "MONGO_URI=mongodb://localhost:27017/task-manager" > .env
echo "PORT=5000" >> .env


Replace MONGO_URI with your MongoDB connection string (e.g., MongoDB Atlas URI or local MongoDB).
Adjust PORT if needed (default is 5000).


Start MongoDB:Ensure MongoDB is running:

Local: Run mongod in a terminal.
Atlas: Ensure your MongoDB Atlas cluster is accessible.


Run the Application:
npm run dev

The API will be available at http://localhost:5000/api/tasks.


Troubleshooting

MongoDB Connection Errors: Check MONGO_URI and ensure MongoDB is running.
Port Conflicts: Change PORT in .env if 5000 is in use.
Dependency Errors: Delete node_modules and package-lock.json, then run npm install again.

