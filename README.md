# 💬 **Chatterly | Full-Stack Real-Time Chat Application.**

**Chatterly** is a production-ready, full-stack real-time chat platform built with the **MERN stack (MongoDB, Express, React, Node.js)**.

Unlike many beginner projects, Chatterly avoids third-party Backend-as-a-Service tools for core functionality. Instead, it implements a **custom Socket.io server** for real-time communication and a **secure JWT-based authentication system**.

---

## 🚀 **Features**

### ⚡ Real-Time Communication
- Instant messaging with **Socket.io**
- Online / offline user indicators
- Typing indicators in real time

### 🔐 Authentication & Security
- Secure **JWT authentication**
- HTTP-only cookies for session safety
- Password hashing using **bcryptjs**
- API rate limiting using **Arcjet**

### 📁 Media & Sharing
- Image uploads and sharing via **Cloudinary**
- Optimized media delivery

### 🎨 User Experience
- Modern UI built with **Tailwind CSS + daisyUI**
- Typing sounds and notification alerts
- Smooth and responsive design

### 📧 Email System
- Automated transactional emails via **Resend**
- Welcome emails on user registration

---

## 🛠️ **Tech Stack**

### 🖥️ Frontend
- **React.js (Vite)**
- **Zustand** – Global state management (auth + chat)
- **Tailwind CSS + daisyUI** – UI styling
- **Lucide-react** – Icons

### ⚙️ Backend
- **Node.js**
- **Express.js**
- **Socket.io** – Real-time engine
- **MongoDB + Mongoose**
- **Cloudinary** – Media storage
- **Arcjet** – Security & rate limiting
- **Resend** – Email service

---

## ⚙️ **Installation & Setup**

### 1️⃣ Clone the repository
```bash
git clone https://github.com/your-username/chatterly.git
cd chatterly
```

### 2️⃣ Install dependencies (root)
```bash
npm run build
```

### 3️⃣ Environment Variables
Create a .env file inside the back-end/ directory:
```bash
# Server
PORT=5000
NODE_ENV=development
CLIENT_URL=http://localhost:3000

# Database
MONGODB_URI=your_mongodb_uri

# Authentication
JWT_SECRET=your_jwt_secret

# Cloudinary (Media Storage)
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

# Arcjet (Security)
ARCJET_KEY=your_arcjet_key
ARCJET_ENV=your_arcjet_environment

# Email Service (Resend)
RESEND_API_KEY=your_resend_api_key
EMAIL_FROM=no-reply@yourdomain.com
EMAIL_FROM_NAME=chatterly
```

### 4️⃣ Run the application
Development mode:
```bash
cd back-end
npm run dev
```

## 🌐 **Deployment**

Chatterly is configured for deployment on any **VPS or platform supporting WebSockets**.

### 🚀 In Production

- **Express** serves the optimized React build from `front-end/dist`
- **Socket.io** runs on the same Node.js server
- Single-domain deployment with **full-stack unified hosting**

---

## 🔐 **Security Highlights**

- **JWT authentication** using HTTP-only cookies  
- **Password hashing** with `bcryptjs`  
- **Rate limiting** powered by Arcjet  
- Secure **environment variable handling**  
- Fully protected **API routes**

---

## 💡 **Why Chatterly?**

Chatterly is designed to demonstrate:

- Real-world **WebSocket architecture**
- Secure **authentication workflows**
- Scalable **MERN monorepo structure**
- Production-level backend practices  
  *(without Backend-as-a-Service shortcuts)*

---

## 📄 **License**

This project is **open-source** and available for learning and personal use.

---

## ❤️ **Author**

Built with passion by **Dulshan Chamika**
