# 📝 Notepad App (Flask + MySQL + Docker)

![Python](https://img.shields.io/badge/Python-3.9-blue?logo=python)
![Flask](https://img.shields.io/badge/Flask-Framework-lightgrey?logo=flask)
![MySQL](https://img.shields.io/badge/MySQL-Database-orange?logo=mysql)
![Docker](https://img.shields.io/badge/Docker-Containerization-2496ED?logo=docker)
![HTML](https://img.shields.io/badge/HTML-Frontend-red?logo=html5)
![CSS](https://img.shields.io/badge/CSS-Styling-blue?logo=css3)

A simple two‑tier **Notepad application** built with:
- **Frontend/Backend:** Python Flask
- **Database:** MySQL (Dockerized)
- **Deployment:** Docker Compose

---

## 📂 Project Structure
``` notepad-app/
├─ app.py                # Flask application
├─ requirements.txt      # Python dependencies
├─ templates/
│    └─ index.html       # HTML frontend
├─ static/
│    └─ style.css        # CSS styling
├─ Dockerfile            # Flask app container
└─ docker-compose.yml    # Multi-container setup
```
## 🚀 Features
- Add notes via a simple web form.
- View all saved notes.
- Delete notes with one click.
- Persistent storage in MySQL.
- Containerized deployment with Docker Compose.
- Healthchecks and restart policies for resilience.

## ⚙️ Setup & Run
  1. Clone the repository
``` 
git clone https://github.com/KailashS3/notepad-app.git
 cd notepad-app
```
  2. Build and start containers
   ```
    docker-compose up --build
  ```
  3. Access the app
```
http://localhost:8080
```

### 🐳 Docker Compose Overview
  - **app:** Flask application container
  - **db:** MySQL 5.7 container with persistent volume
  - **network:** Bridge network for communication
  - **restart policy:** always
  - **healthchecks:** ensure both containers are alive

## 🔧 Configuration
Database connection details are set directly in app.py
```
DB_HOST = "db"
DB_USER = "root"
DB_PASSWORD = "rootpass"
DB_NAME = "notesdb"
```

## 📸 Demo Screenshot
**Add notes**

<img width="400" height="280" alt="image" src="https://github.com/user-attachments/assets/9b12e10c-1ed8-45b4-8c30-3b34912fda0f" />

**Delete note "Deleting it"**

<img width="400" height="240" alt="image" src="https://github.com/user-attachments/assets/d5497c31-1439-42fb-adf6-9df890987e44" />


