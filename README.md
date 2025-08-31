Job Portal

A full-stack Job Portal application where users can register, browse jobs, apply for positions, and companies can post job openings. Built with a React frontend, Node.js/Express backend, and MongoDB for database management. Supports user authentication, role-based access, and file uploads via Cloudinary.

Features
For Users

User registration and login (with JWT authentication)

Browse available jobs

Apply for jobs

View application status

Upload profile images/resumes

For Companies

Company registration and login

Post new job listings

Manage job postings

View applicants for posted jobs

Common

Role-based access control (User / Company)

Secure password hashing with bcrypt

Cloudinary integration for file storage (profile images, resumes)

RESTful APIs for frontend-backend communication

Tech Stack

Frontend: React.js, Tailwind CSS

Backend: Node.js, Express.js

Database: MongoDB

Authentication: JWT

File Storage: Cloudinary

Other Tools: Postman for API testing, Nodemon for development

Installation
Backend

Navigate to the backend folder:

cd backend


Install dependencies:

npm install


Create a .env file and add the following environment variables:

PORT=8000
MONGO_URI=<Your MongoDB Connection String>
JWT_SECRET=<Your JWT Secret>
CLOUDINARY_CLOUD_NAME=<Cloudinary Cloud Name>
CLOUDINARY_API_KEY=<Cloudinary API Key>
CLOUDINARY_API_SECRET=<Cloudinary API Secret>


Start the backend server:

npm run dev

Frontend

Navigate to the frontend folder:

cd frontend


Install dependencies:

npm install


Start the frontend development server:

npm start


Open http://localhost:3000
 in your browser.

API Endpoints

User: /api/v1/user

Job: /api/v1/job

Application: /api/v1/application

Company: /api/v1/company

(Refer to Postman collection or backend routes for full API details.)

Folder Structure
backend/
├─ models/       # Mongoose models
├─ controllers/  # Request handlers
├─ routes/       # API routes
├─ utils/        # Utilities (Cloudinary, Data URI, etc.)
├─ server.js     # Entry point

frontend/
├─ src/
│  ├─ components/  # Reusable UI components
│  ├─ pages/       # Application pages
│  ├─ api/         # API calls
│  ├─ App.js
│  └─ index.js
