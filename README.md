# 🎓 StudyNotion

StudyNotion is a full-stack ed-tech platform where instructors can create, manage, and sell courses, while students can browse, purchase, and track their learning progress. It integrates modern technologies and tools to deliver a seamless and efficient learning experience.

---

## 🚀 Features

### 👨‍🏫 For Instructors:
- Instructor registration and login
- Course creation with modular structure (Sections & Subsections)
- Video upload and hosting via **Cloudinary**
- Course publishing/unpublishing
- Revenue and enrollment insights

### 👨‍🎓 For Students:
- Student registration and login
- Explore all available courses
- Secure course purchasing via **Razorpay**
- Access course content post-purchase
- Track progress through completed subsections
- Update profile, view enrolled courses

### 🔐 Authentication & Authorization:
- Role-based access control (Student, Instructor, Admin)
- JWT-based authentication
- Protected routes using middleware in **Express.js**

---

## 🛠️ Tech Stack

### Frontend:
- React.js (with **Vite**)
- Redux Toolkit for state management
- Tailwind CSS for UI styling
- React Router for navigation
- Toast notifications using **react-hot-toast**

### Backend:
- Node.js & Express.js
- MongoDB with Mongoose
- Cloudinary (for media storage)
- Razorpay (for payment gateway)
- dotenv (for environment configuration)
- JWT for authentication
- bcrypt.js for password hashing

---

![Screenshot 2025-05-02 101147](https://github.com/user-attachments/assets/c907f819-33a9-4fe3-8465-3c97e405a7ea)

---
## 🔧 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/studynotion.git
cd StudyNotion
```

# 🚀 Running StudyNotion with Docker

StudyNotion is fully containerized using **Docker**, allowing you to run the full application (Frontend + Backend + MongoDB) with a single command.

---

## 📦 Prerequisites

- Install **Docker Desktop**  
  👉 https://www.docker.com/products/docker-desktop/

- Clone the repository:

```bash
git clone https://github.com/your-username/StudyNotion.git
cd StudyNotion
```

▶️ Start Application Using Docker
In the project root (where docker-compose.yml exists), run:

```bash
docker compose up -d --build
```

This will:
Build and start the frontend
Build and start the backend
Start MongoDB
Connect all containers automatically

🌍 Access the Application
Service	URL	Description
Frontend	http://localhost:5173	React App (Nginx)
Backend API	http://localhost:4000/api/v1	Express API
MongoDB	localhost:27016	Database

🔁 Restart Services
```bash
docker compose restart
```

🛑 Stop All Containers
```bash
docker compose down
```

🧹 Full Cleanup (Images + Containers + Volumes)
```bash
docker compose down --rmi all --volumes
```

🛠️ Running Without Docker (Local Setup)
1️⃣ Backend Setup

```bash
cd server
npm install
```

Create .env inside /server: .env.example are given for sample

Start backend:

```bash
npm run start
```

2️⃣ Frontend Setup

```bash
cd ../frontend
npm install
```

Create .env inside /frontend: .env.example are given for sample
Start frontend:

```bash
npm run dev
```

🎉 That's it!
Your StudyNotion application is now fully set up and running — either with Docker (recommended) or locally for development.