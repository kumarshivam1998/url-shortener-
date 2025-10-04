URL Shortener<br />
A full-stack URL shortener application built with React, Express, and MongoDB. Users can create short links, register/login, and track their URLs and click counts.<br />

<img alt="Screenshot" src="https://github.com/user-attachments/assets/20d14cf4-f346-41d9-b184-568880c1b355">

Features<br />
-- Shorten long URLs with or without authentication<br />
-- Custom short URLs for registered users<br />
-- User registration and login (JWT-based authentication)<br />
-- Dashboard to view and copy your URLs and click stats<br />
-- Responsive UI built with React and TailwindCSS<br />
-- RESTful API with Express and MongoDB<br />
Tech Stack<br />
-- Frontend: React, TailwindCSS, Redux Toolkit, TanStack Query, TanStack Router, Axios, Vite<br />
-- Backend: Express, MongoDB, Mongoose, JWT, NanoID, bcryptjs<br />
-- Other: dotenv, cookie-parser, cors<br />
Getting Started<br />
1. Clone the repository <br />
git clone https://github.com/yourusername/urlshortener.git<br />
cd urlshortener<br />
2. Backend Setup<br />
cd backend<br />
npm install<br />
-- Create a .env file in the backend folder:<br />
MONGO_URI=your_mongodb_connection_string<br />
APP_URL=http://localhost:3000/<br />
JWT_SECRET=your_jwt_secret<br />
-- Start the backend server:<br />
npm run dev<br />
or<br />
npm start<br />
3. Frontend Setup<br />
cd frontend<br />
npm install<br />
npm run dev<br />
The frontend will run on http://localhost:5173<br />
4. MongoDB Setup<br />
-- Make sure you have a MongoDB instance running and update MONGO_URI in your .env file.<br />
Usage<br />
Visit http://localhost:5173 in your browser.<br />
-- Register or login to create custom short URLs and view your dashboard.<br />
-- Unauthenticated users can still shorten URLs, but won’t have access to dashboard features.<br />

Folder Structure<br />
urlshortener/<br />
  backend/<br />
    app.js<br />
    src/<br />
      config/<br />
      controller/<br />
      dao/<br />
      middleware/<br />
      models/<br />
      routes/<br />
      services/<br />
      utils/<br />
    .env<br />
    package.json<br />
  frontend/<br />
    src/<br />
      api/<br />
      components/<br />
      pages/<br />
      routing/<br />
      store/<br />
      utils/<br />
      main.jsx<br />
      index.css<br />
    public/<br />
    package.json<br />
    vite.config.js<br />

------------------<br />



API Endpoints<br />
POST /api/create – Create a short URL<br />
POST /api/auth/register – Register a new user<br />
POST /api/auth/login – Login<br />
POST /api/auth/logout – Logout<br />
GET /api/auth/me – Get current user<br />
POST /api/user/urls – Get all URLs for the logged-in user<br />
GET /:id – Redirect to the original URL<br />

License<br />
MIT<br />
