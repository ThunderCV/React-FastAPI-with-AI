# Secure-AI-App-With-Auth

An end-to-end **full-stack AI-powered application** with authentication.
This project demonstrates a **FastAPI backend** with AI utilities, **Clerk for authentication**, **Grok webhooks**, and a **React + Vite frontend** for the user interface.

---

## 📂 Project Structure

```
Secure-AI-App-With-Auth/
├── frontend/              # React + Vite frontend
│   ├── public/            # Static assets
│   ├── src/               # React components & styles
│   ├── package.json       # Frontend dependencies
│   └── vite.config.js     # Vite configuration
│
├── backend/               # FastAPI backend
│   ├── src/               # Application logic
│   │   ├── app.py         # Main FastAPI app
│   │   ├── ai_generator.py# AI generation module
│   │   └── utils.py       # Helper utilities
│   ├── server.py          # Uvicorn entrypoint
│   ├── pyproject.toml     # Python dependencies
│   └── database.db        # SQLite database
│
├── .venv/                 # Virtual environment
├── .git/                  # Git repository
├── .idea/                 # PyCharm project settings
└── README.md              # Project documentation
```

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/<your-username>/Secure-AI-App-With-Auth.git
cd Secure-AI-App-With-Auth
```

---

### 2️⃣ Backend Setup (FastAPI + Uvicorn)

1. Navigate to backend:

   ```bash
   cd backend
   ```

2. Create & activate a virtual environment:

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

   *(or use `uv` if you prefer modern dependency management)*

4. Run the server:

   ```bash
   uvicorn server:app --reload
   ```

   Backend runs at: **[http://127.0.0.1:8000](http://127.0.0.1:8000)**

---

### 3️⃣ Frontend Setup (React + Vite)

1. Navigate to frontend:

   ```bash
   cd frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Run the development server:

   ```bash
   npm run dev
   ```

   Frontend runs at: **[http://localhost:5173](http://localhost:5173)**

---

## 🔑 Features

* ✅ Secure authentication flow powered by **Clerk**
* ✅ FastAPI backend with AI utilities (`ai_generator.py`)
* ✅ Grok integration for **webhook handling**
* ✅ React + Vite frontend for UI
* ✅ SQLite database integration
* ✅ Modular architecture (backend + frontend separation)

---

## 🛠 Tech Stack

* **Backend**: FastAPI, SQLAlchemy, Uvicorn
* **Frontend**: React, Vite, Tailwind (if used)
* **Database**: SQLite (default, can be replaced)
* **Authentication**: Clerk
* **Webhooks**: Grok
* **AI**: OpenAI / custom AI module (`ai_generator.py`)

---

## 📜 License

This project is licensed under the **MIT License** – feel free to use and adapt.
