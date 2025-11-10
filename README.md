# VueJS-Flask-Game-Library

A full-stack web application for managing a simple **game library**, built with Vue.js (frontend) and Flask (backend). This project is ideal for demonstrating modern frontend (Vue.js) and backend (Flask) development skills.

---

## 📚 About The Project

This app lets users perform CRUD (Create, Read, Update, Delete) operations on a game library. Games have properties like `title`, `genre`, and `played`. The frontend is built using Vue.js 2, and it communicates with a Python Flask REST API.

---

## 🧰 Tech Stack

- **Frontend:** Vue.js 2, Axios, Bootstrap/Bootswatch for UI
- **Backend:** Python 3.9, Flask, Flask-CORS
- **Build Tools:** npm, Babel
- **Other:** RESTful API, Component-based architecture, CORS for dev environment

---

## 🗂️ Project Structure

VueJS-Flask-Game-Library/
│
├── backend/
│ ├── main.py # Flask API: routes for games CRUD, logic
│ ├── Pipfile # Python dependencies (Flask, Flask-Cors)
│ ├── Pipfile.lock # Locked dependencies
│ └── requirements.txt # (Optional) Python dependencies
│
├── frontend/
│ ├── public/
│ │ ├── favicon.ico
│ │ └── index.html # Root HTML file for Vue app
│ ├── src/
│ │ ├── assets/
│ │ │ └── logo.png
│ │ ├── components/
│ │ │ ├── Games.vue # Main game library component
│ │ │ ├── HelloWorld.vue # Starter component
│ │ │ └── Shark.vue # Additional sample
│ │ ├── router/
│ │ ├── App.vue # Root app component
│ │ └── main.js # Vue entry point
│ ├── .gitignore
│ ├── babel.config.js
│ ├── package.json # Node dependencies
│ ├── package-lock.json
│ └── README.md 
│
├── plan.txt # Project planning notes
├── README.md 


---

## 🌟 Features

- **Game Library CRUD:** Add, edit, delete, view games
- **RESTful API:** Flask backend with routes to handle GET, POST, PUT, DELETE
- **Responsive UI:** Uses Bootstrap for clean, modern design
- **Vue.js Component Architecture:** Separation of concerns, single-file components
- **Modal Forms:** Uses modals for game creation and updates
- **Status Alerts:** User feedback on actions (success, validation, etc.)

---

## 🚦 Workflow

**Frontend Vue.js**
- Makes HTTP requests to Flask API (`localhost:5000`)
- Components handle displaying and editing game data
- State managed locally, refreshed after API operations

**Backend Flask**
- Stores games in-memory (can be extended to use a DB)
- Handles requests for:
  - `/games` (GET: list all, POST: add game)
  - `/games/<game_id>` (PUT: update game, DELETE: remove game)
- Uses CORS to allow local Vue.js development

---

## 🚀 Getting Started

### Prerequisites

- Python (>= 3.9)
- Node.js & npm (for frontend)
- Git

### Backend Setup

cd backend

Install Python dependencies
pip install flask flask-cors

or use pipenv
pipenv install

Run backend server
python main.py


### Frontend Setup

cd frontend
npm install
npm run serve


> The Vue app will run on a certain port (usually `8080`), and the Flask server runs on `5000`. Make sure both are running when you use the app.

---

## 🔗 API Overview

- `GET /games` — get all games
- `POST /games` — add a game (`title`, `genre`, `played`)
- `PUT /games/<game_id>` — update a game
- `DELETE /games/<game_id>` — delete a game

---


---

## 📝 Contributing

Fork the repo, open PRs, or issues with suggestions!

---

