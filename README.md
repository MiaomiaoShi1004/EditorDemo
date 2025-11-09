# Online Text Editor | EditorDemo

This is a collaborative online text editor built with **React**, **Node.js**, **Express**, and **Socket.io**. It supports real‑time editing using WebSockets and basic document sharing via email (email functionality is currently unfinished).

---

## 🚀 Run Locally

### 1. Clone the project
```bash
git clone [xxxx](https://github.com/MiaomiaoShi1004/EditorDemo)
cd EditorDemo
```

### 2. Install dependencies
Install all dependencies in the three main directories:
```bash
cd client
npm install
cd ../server
npm install
cd ../socket
npm install
```

### 3. Create your `.env` file
Inside the `server` directory, create a file named `.env` with the following variables:

```env
MONGO_URI=mongodb://localhost:27017/editordemo
PORT=8080
JWT_SECRET=supersecretlocalkey
JWT_LIFETIME=1d
SMTP_FROM_EMAIL=test@example.com
SMTP_FROM_PASSWORD=testpassword
```

> Note: You can use dummy values for the SMTP settings. Email functionality is optional and currently not fully implemented.

### 4. Start each service
Open three terminal tabs and run:

**Backend (API server)**
```bash
cd server
npm start
```

**Socket server**
```bash
cd socket
npm start
```

**Frontend (client)**
```bash
cd client
npm run dev
```

### 5. Open the app
Once the client is running, open the printed URL (usually `http://localhost:5173`) in your browser.

- The backend runs on **http://localhost:8080**
- The socket server runs on **ws://localhost:3000**

---

## 🧠 Tech Stack
- **Frontend:** React, Redux, TailwindCSS, Redux‑persist  
- **Backend:** Node.js, Express, MongoDB, Socket.io, Nodemailer  

---

### 📝 Notes
- The main feature is the **real‑time collaborative text editing** using WebSockets.  
- The **email sharing** feature exists but is not fully reliable — it’s mostly a proof of concept.  
- This project serves as a base demo for extending real‑time collaboration functionality.

