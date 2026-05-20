🚀 Task Manager Pro  
A modern **MERN stack** productivity platform featuring **personal task management, team collaboration, admin controls, email invites, and real-time notifications**.

---

## ⭐ Key Features

### 🔐 **Authentication & Security**
- JWT Authentication with **HTTP-only cookies**  
- Protected API routes (backend)  
- Protected UI routes (frontend)  
- Role-based access: **user / admin**  
- Validation + secure password hashing

---

## 📝 Personal Task Management
- Create, edit, delete tasks  
- Soft delete (Trash Bin)  
- Restore or permanently delete  
- Priority levels + due dates  
- Mark complete/pending  
- Filters (completed, pending, high priority)

---

## 👥 Team Collaboration System
- Create teams  
- Roles: **owner / admin / member**  
- Add or remove members  
- Email invites for new members (Nodemailer)  
- Team-specific tasks  
- Task workflow: **Todo → In Progress → Done**  
- Assign tasks to members  
- Permission system for who can edit/delete tasks

---

## 🔔 Real-Time Notifications (Socket.IO)
- Live notifications for:
  - Team invites  
  - Member removal  
  - New task added  
  - Assignment updates  
- No refresh required  
- In-app notification dropdown  
- Unread badge counter

---

## 🛡 Admin Dashboard
Admin panel with full system control:  
- View all users  
- Delete users (with task cleanup)  
- View all tasks  
- Permanent delete  
- System analytics  
  - Total users  
  - Total tasks  
  - Completed vs Pending  
  - Daily task creation stats (chart-ready)

---

## 📊 Advanced Features
- Modular, scalable backend architecture  
- Clean folder structure  
- Reusable UI components with TailwindCSS  
- Team task board (Kanban-style grouping)  
- Fully responsive design (mobile-ready)

---

## 🏗 Tech Stack

### **Frontend**
- React + Vite  
- Tailwind CSS  
- Axios  
- React Router  
- Socket.IO Client  

### **Backend**
- Node.js  
- Express.js  
- MongoDB + Mongoose  
- JWT Auth  
- Nodemailer  
- Socket.IO (real-time communication)  

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repo
```bash
git clone https://github.com/jatinvaid108/TaskManager-app.git
cd project-folder

2️⃣ Setup Backend (server/)

Create .env inside /server:

PORT=5000
MONGO_URI=your_mongodb_url
JWT_SECRET=your_secret_key
JWT_EXPIRES_IN=7d

EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password
EMAIL_FROM="Task Manager Pro <your_email@gmail.com>"

Then install backend dependencies:

cd server
npm install
npm run dev

Backend runs at:
👉 http://localhost:5000

3️⃣ Setup Frontend (client/)

Create .env inside /client:

VITE_API_BASE_URL=http://localhost:5000/api
VITE_SOCKET_URL=http://localhost:5000

Install Dependencies
cd client
npm install
npm run dev

Frontend runs at:
👉 http://localhost:5173

🚀 Deployment Ready

Works with Render / Vercel / Netlify

Environment variables supported

Handles CORS + cookies correctly

Socket.IO integrated for production

📁 Project Structure
project/
│
├── server/
│   ├── controllers/
│   ├── models/
│   ├── middleware/
│   ├── routes/
│   ├── utils/
│   ├── src/server.js (Socket.IO server)
│   └── app.js
│
└── client/
    ├── src/
    │   ├── pages/
    │   ├── components/
    │   ├── teams/
    │   ├── admin/
    │   ├── context/
    │   ├── utils/
    │   └── App.jsx


❤️ Author
Nainy Bansal
Full-Stack Developer | MERN | Real-Time Apps | System Design

⭐ Support

If you like the project, please ⭐ the repository!
