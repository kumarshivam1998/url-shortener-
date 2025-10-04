URL Shortener
A full-stack URL shortener application built with React, Express, and MongoDB. Users can create short links, register/login, and track their URLs and click counts.

<img alt="Screenshot" src="https://github.com/user-attachments/assets/20d14cf4-f346-41d9-b184-568880c1b355">

Features
-- Shorten long URLs with or without authentication
-- Custom short URLs for registered users
-- User registration and login (JWT-based authentication)
-- Dashboard to view and copy your URLs and click stats
-- Responsive UI built with React and TailwindCSS
-- RESTful API with Express and MongoDB
Tech Stack
-- Frontend: React, TailwindCSS, Redux Toolkit, TanStack Query, TanStack Router, Axios, Vite
-- Backend: Express, MongoDB, Mongoose, JWT, NanoID, bcryptjs
-- Other: dotenv, cookie-parser, cors
Getting Started
1. Clone the repository
git clone https://github.com/yourusername/urlshortener.git
cd urlshortener
2. Backend Setup
cd backend
npm install
-- Create a .env file in the backend folder:
MONGO_URI=your_mongodb_connection_string
APP_URL=http://localhost:3000/
JWT_SECRET=your_jwt_secret
-- Start the backend server:
npm run dev
# or
npm start
3. Frontend Setup
cd frontend
npm install
npm run dev
The frontend will run on http://localhost:5173
4. MongoDB Setup
-- Make sure you have a MongoDB instance running and update MONGO_URI in your .env file.
Usage
Visit http://localhost:5173 in your browser.
-- Register or login to create custom short URLs and view your dashboard.
-- Unauthenticated users can still shorten URLs, but won’t have access to dashboard features.

Folder Structure
urlshortener/
  backend/
    app.js
    src/
      config/
      controller/
      dao/
      middleware/
      models/
      routes/
      services/
      utils/
    .env
    package.json
  frontend/
    src/
      api/
      components/
      pages/
      routing/
      store/
      utils/
      main.jsx
      index.css
    public/
    package.json
    vite.config.js

------------------



API Endpoints
POST /api/create – Create a short URL
POST /api/auth/register – Register a new user
POST /api/auth/login – Login
POST /api/auth/logout – Logout
GET /api/auth/me – Get current user
POST /api/user/urls – Get all URLs for the logged-in user
GET /:id – Redirect to the original URL

License
MIT
