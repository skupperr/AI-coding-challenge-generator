<div align="center">

# 🧠 AI Coding Challenge Generator

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![Python 3.11+](https://img.shields.io/badge/Python--3.11+-backend-blue?logo=python)](https://www.python.org/downloads/)
[![Vite + React](https://img.shields.io/badge/Vite_+_React-frontend-purple?logo=react)](https://vitejs.dev/)

> Practice makes perfect — sharpen your coding skills with daily AI-generated MCQs.

**AI Coding Challenge Generator** is a full-stack application that helps users improve their coding skills through daily AI-generated multiple-choice challenges, tailored by difficulty.

![Demo Screenshot](./Frontend/public/preview.png)

</div>

## 🚀 Features

- 🧠 **AI-Generated Coding Questions**: Challenges are created using a local Ollama LLM model.
- 🔐 **Authentication with Clerk**: Users must log in to access the platform.
- 🎯 **Difficulty-Based Challenges**: Choose from multiple difficulty levels.
- 📊 **MCQ Format**: All challenges are multiple choice for quick practice and validation.
- 📅 **Daily Quota System**: Users can attempt a limited number of challenges per day, which resets every 24 hours.
- 🕘 **History Tracking**: All past challenges are stored in a secure SQLAlchemy database.

---

## 🛠️ Tech Stack

### Frontend
[![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&color=2d2d2d)](https://react.dev/)
[![JavaScript](https://img.shields.io/badge/javascript-61DAFB?style=for-the-badge&logo=javascript&color=2d2d2d)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&color=2d2d2d)](https://vitejs.dev/)
[![Clerk](https://img.shields.io/badge/Clerk-6C47FF?style=for-the-badge&logo=clerk&color=2d2d2d)](https://clerk.dev/)

### Backend
[![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=for-the-badge&logo=python&labelColor=2d2d2d)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&color=2d2d2d)](https://fastapi.tiangolo.com/)
[![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-cc0000?style=for-the-badge&logo=sqlite&color=2d2d2d)](https://www.sqlalchemy.org/)
[![Clerk SDK](https://img.shields.io/badge/Clerk_Backend-6C47FF?style=for-the-badge&logo=clerk&color=2d2d2d)](https://clerk.dev/)
[![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=OpenAI&color=2d2d2d)](https://ollama.com/)

---

## 🔍 How It Works

1. **User logs in** via Clerk.
2. After login, user selects a **difficulty level** (e.g., Easy, Medium, Hard).
3. A **local Ollama model** generates a multiple-choice coding challenge.
4. The challenge is shown on the frontend and **stored in the backend** database.
5. A **daily quota** system ensures users can only attempt a limited number per day.
6. Once the quota resets, the user can generate more challenges.

---

## 💻 How to Use This Repo


### 1. Clone the repository
```bash
git clone https://github.com/skupperr/AI-Coding-Challenge-Generator.git
cd AI-Coding-Challenge-Generator
```
### 2. Set up the frontend
```bash
cd Frontend
npm install
npm run dev
```
### 3. In a new terminal, set up the backend
```bash
cd ../Backend
pip install -r requirements.txt
python server.py
```

---

## 👥 Who Is It For?

- **👨‍💻 Developers**: Looking to sharpen their coding skills with AI-generated practice.
- **📚 Students**: Practice MCQs before technical interviews or exams.
- **🧠 Lifelong Learners**: Anyone who wants a quick daily coding brain-teaser.

---

## 📁 Project Structure

```
AI-Coding-Challenge-Generator/
├── Backend/ # FastAPI backend
│ ├── src/
│ │ ├── routes/
│ │ ├── models/
│ │ ├── database/
│ │ ├── ai_generator.py
│ │ ├── app.py
│ │ ├── utils.py
│ │ └── .env
│ ├── server.py
│ └── requirements.txt
│
├── Frontend/ 
│ ├── src/
│ │ ├── auth/
│ │ ├── challenges/
│ │ ├── history/
│ │ ├── layout/
│ │ ├── utils/
│ │ ├── App.css
│ │ ├── index.css
│ │ ├── main.jsx
│ │ ├── App.jsx
│ ├── public/
│ ├── .env
│ ├── index.html
│ └── package.json
│
└── README.md
```

## 📬 Contact

Created with ❤️ by [Asif U. Ahmed](https://github.com/skupperr)

[Report Bug](https://github.com/skupperr/AI-Coding-Challenge-Generator/issues) · [Request Feature](https://github.com/skupperr/AI-Coding-Challenge-Generator/issues)