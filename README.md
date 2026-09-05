# CoffeE ☕

A full-stack e-commerce web application for coffee products, built with the **MERN stack** (MongoDB, Express, React, Node.js) and Tailwind CSS.

Includes an admin dashboard, product management, user authentication, order management, and sentiment-based product recommendations.

## Features

- Modern, responsive UI (React + Tailwind CSS)
- Product catalog with search and filtering
- Product details with reviews and sentiment analysis
- Shopping cart and checkout flow
- User registration, login, and profile management
- Admin dashboard: manage products, orders, users, and subscriptions
- Order placement, payment method selection, and delivery tracking
- Sentiment-based product recommendations (NLP with `natural`)
- TF-IDF analysis for product content
- RESTful API (Express.js)
- MongoDB for data storage

## Folder Structure

backend/ # Node.js / Express API, MongoDB models, controllers
frontend/ # React app (Vite), Tailwind CSS, components, pages
uploads/ # Uploaded product images

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- MongoDB database (local or cloud, e.g. MongoDB Atlas)

### 1. Clone the repository

```bash
git clone https://github.com/KritanDotel69/CoffeE.git
cd CoffeE
```

2. Backend Setup
   cd backend
   npm install

# Create a .env file

cp .env.example .env

# Edit .env with your MongoDB URI and JWT secret

npm run dev 3. Frontend Setup
cd ../frontend
npm install

# Create a .env file

cp .env.example .env

# Set VITE_BACKEND_URL to your backend URL

npm run dev

4. Seed the Database
   cd backend
   node seeder.js

5. Production Build

# In frontend

npm run build

# Environment Variables

Backend (.env)
envMONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
NODE_ENV=development
PORT=5000

Frontend (.env)
envVITE_BACKEND_URL=http://localhost:5000

# Tech Stack

Frontend: React, Vite, Tailwind CSS, Redux Toolkit, React Router, Chart.js
Backend: Node.js, Express.js
Database: MongoDB + Mongoose
Auth: JWT
NLP: natural (sentiment analysis & TF-IDF)

# Deployment

You can deploy the backend and frontend separately (e.g. Render + Vercel/Netlify) or as a single full-stack app.
Make sure to set all required environment variables in your hosting platform.

CoffeE — Modern coffee e-commerce with smart recommendations and admin control.
