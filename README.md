# React Barely Social Project (Frontend + Backend)

This repository contains a **fullstack project** using **Git submodules**.

- `client/` → Frontend (separate Git repository)
- `server/` → Backend (separate Git repository)

Both are linked together in this repo for easy setup and sharing.

---

## 📦 Project Structure

```
fullstack-project/
├── client/   # Frontend (submodule)
├── server/   # Backend (submodule)
├── .gitmodules
└── README.md
```

---

## 🚀 How to Clone the Project (IMPORTANT)

You **must** clone this repo with submodules.

### ✅ Correct Way (Recommended)

```bash
git clone --recurse-submodules https://github.com/your-username/fullstack-project.git
```

### ❌ Wrong Way (Will NOT download frontend/backend)

```bash
git clone https://github.com/your-username/fullstack-project.git
```

If you already cloned the wrong way, fix it by running:

```bash
git submodule update --init --recursive
```

---

## 🖥️ How to Run the Project

### 1️⃣ Start Backend

```bash
cd server
npm install
npm start
```

> Make sure backend is running before starting frontend.

---

### 2️⃣ Start Frontend

Open a new terminal:

```bash
cd client
npm install
npm run dev
```

(Use `npm start` if your frontend uses CRA)

---

## ⚙️ Requirements

- Node.js (v16+ recommended)
- npm
- Git

---

## 📝 Important Notes

- `client` and `server` are **Git submodules**
- Do NOT delete the `.gitmodules` file
- Do NOT commit frontend/backend changes from the root folder

---

## 🧑‍💻 For Contributors / Developers

### Making changes

#### Frontend changes

```bash
cd client
git add .
git commit -m "Frontend update"
git push
```

#### Backend changes

```bash
cd server
git add .
git commit -m "Backend update"
git push
```

#### Update main repo reference

```bash
cd ..
git add client server
git commit -m "Update submodule pointers"
git push
```

---

## 🧠 One-line Explanation

> This repo manages frontend and backend as **linked repositories**, not copied code.

---

## 📌 Access Note

To fully clone this project, you must have access to:

- the frontend repository
- the backend repository

If either repo is private, request collaborator access.
