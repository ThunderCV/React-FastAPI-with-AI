# Secure-AI-App-With-Auth

An end-to-end **full-stack AI-powered application** with authentication.
This project demonstrates a **FastAPI backend** with AI utilities, **Clerk for authentication**, **ngrok for webhook tunneling**, and a **React + Vite frontend** for the user interface.

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

### 4️⃣ Clerk Authentication Setup

1. Create a Clerk account at [https://clerk.com](https://clerk.com)
2. Copy your **Frontend API Key** and **JWT templates**.
3. Add them to your `.env` files in both **frontend** and **backend**.
4. Frontend automatically integrates Clerk UI components for sign-in/sign-up.

---

### 5️⃣ Ngrok for Webhooks

Use **ngrok** to expose your local FastAPI backend for webhook testing.

1. Install ngrok:

   ```bash
   brew install ngrok
   ```

   *(or download from [https://ngrok.com/download](https://ngrok.com/download))*

2. Run ngrok on port 8000:

   ```bash
   ngrok http 8000
   ```

3. Copy the generated public URL and register it as your **webhook URL** in Clerk or other external services.

---

## 🔑 Features

* ✅ Secure authentication flow powered by **Clerk**
* ✅ FastAPI backend with AI utilities (`ai_generator.py`)
* ✅ **ngrok integration for webhook tunneling**
* ✅ React + Vite frontend for UI
* ✅ SQLite database integration
* ✅ Modular architecture (backend + frontend separation)

---

## 🛠 Tech Stack

* **Backend**: FastAPI, SQLAlchemy, Uvicorn
* **Frontend**: React, Vite, Tailwind (if used)
* **Database**: SQLite (default, can be replaced)
* **Authentication**: Clerk
* **Webhooks**: ngrok
* **AI**: OpenAI / custom AI module (`ai_generator.py`)

---

## 📜 License

This project is licensed under the **MIT License** – feel free to use and adapt.
