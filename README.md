# AWKUM Chatbot

This project features a Python backend built with FastAPI and a modern React frontend powered by Vite.

## 📋 Prerequisites

Before running the application, make sure you have the following installed on your system:
- [Python 3.10+](https://www.python.org/downloads/)
- [Node.js 18+](https://nodejs.org/)
- [Git](https://git-scm.com/)
- [MongoDB](https://www.mongodb.com/try/download/community) (Make sure the MongoDB service is running locally or provide a connection URI in `.env`)

---

## ⚙️ Environment Variables

Create a file named `.env` in the root folder (where `main.py` is located) and configure it based on your external services (like Google GenAI, Groq, database string, etc.):

```env
# Example .env file mapping
GROQ_API_KEY=your_groq_api_key
GOOGLE_API_KEY=your_google_api_key
MONGO_URI=mongodb://localhost:27017
```

---

## 🐧 Setup on Linux (Ubuntu / Debian)

### 1. Backend Setup

Open a terminal and run the following commands:

```bash
# 1. Navigate to the root directory of the project
cd /path/to/Chatbot

# 2. Create a Python virtual environment
python3 -m venv venv

# 3. Activate the virtual environment
source venv/bin/activate

# 4. Install backend dependencies
pip install -r requirements.txt

# 5. Start the backend server
uvicorn main:app --reload
```
The FastAPI backend will now be available at: **http://127.0.0.1:8000**

### 2. Frontend Setup

Open a **new** terminal window and run:

```bash
# 1. Navigate to the frontend directory
cd /path/to/Chatbot/frontend

# 2. Install Node dependencies
npm install

# 3. Start the Vite development server
npm run dev
```
The React frontend will be available at: **http://localhost:5173** (or the port specified in your terminal).

---

## 🪟 Setup on Windows

### 1. Backend Setup

Open **Command Prompt** or **PowerShell** as an administrator (if required) and run:

```cmd
:: 1. Navigate to the root folder (adjust path accordingly)
cd path\to\Chatbot

:: 2. Create a Python virtual environment
python -m venv venv

:: 3. Activate the virtual environment
.\venv\Scripts\activate

:: 4. Install backend dependencies
pip install -r requirements.txt

:: 5. Start the backend server
uvicorn main:app --reload
```
The FastAPI backend will now be available at: **http://127.0.0.1:8000**

### 2. Frontend Setup

Open a **new** Command Prompt or PowerShell window:

```cmd
:: 1. Navigate to the frontend directory
cd path\to\Chatbot\frontend

:: 2. Install Node dependencies
npm install

:: 3. Start the Vite development server
npm run dev
```
The React frontend will be available at: **http://localhost:5173**

---

## 📖 API Documentation

FastAPI automatically generates interactive API documentation. While the backend is running, visit:
- **Swagger UI:** `http://127.0.0.1:8000/docs`
- **ReDoc:** `http://127.0.0.1:8000/redoc`

Happy Coding! 🚀
