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
