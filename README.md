# 📝 Notes App

A simple and efficient Notes Application that allows users to create, edit, delete, pin and manage notes in a clean interface.  
The project focuses on CRUD operations, UI usability, and real-world application structure.

---

## 📌 Features
- ➕ Create new notes
- ✏️ Edit existing notes
- 🗑️ Delete notes
- 🔍 Search notes
- 📌 Pin notes
- 💾 Create folder
- 📱 Responsive UI (works on mobile & desktop)

---

## 🎯 Purpose
This project was built to practice:
- Frontend development
- State management
- CRUD operations
- Client-side storage
- Application structure & modular coding

It simulates a real productivity tool similar to Google Keep or Apple Notes.

---

Project Structure
client: React Frontend
server: Express Backend
server/database.sqlite: Auto-generated database file (after first run)

---

## 🛠️ Tech Stack

### Frontend
- React (Vite)
- Tailwind CSS
- React Router
- React Hook Form
- Axios
- Lucide React

### Backend
- Node.js
- Express
- SQLite (sqlite3/sqlite wrapper)
- PDF/JWT Auth

### Database
- SQLite (Local file-based database for zero-config setup)

Setup Steps

### Prerequisites
Node.js (v16+)
npm

### 🛠️ Backend Setup
bash
cd server
npm install
npm start

Server runs on http://localhost:5000
Creates database.sqlite automatically.

### 🛠️ Frontend Setup
Open a new terminal:
bash
cd client
npm install
npm run dev

Frontend runs on http://localhost:5173

### 📱 Demo Credentials
(You can sign up with any email, but here is a pre-seeded example if you wish)
Email: demo@example.com
Password: password123

### How would you scale this for production?
To scale this application for production:
1.Database: Migrate from SQLite to a managed PostgreSQL or MongoDB cluster (e.g., AWS RDS or MongoDB Atlas) for concurrency and reliability. Add Redis for caching frequent queries (e.g., fetching user profile).
2.API: Vertical scaling initially, then horizontal scaling using a Load Balancer (Nginx/AWS ELB) with multiple Node.js instances (PM2 cluster mode).
3.Frontend: Build static assets and serve via a CDN (Cloudfront/Vercel) for global low latency.
4.Security: Enforce HTTPS, add Rate Limiting (express-rate-limit), and use HTTP-only cookies for JWT storage instead of LocalStorage to prevent XSS.

### API Documentation
See postman_collection.json for the full API spec.

---

## 📸 Screenshots

### Home Page

