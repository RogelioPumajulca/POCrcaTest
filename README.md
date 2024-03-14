# PoC 2024 - GUI

RCA Module

#### Authors
 Rogelio Pumajulca

## Directory Structure
- `frontend`: Vue.js frontend code, static files <-- not anymore :b
- `backend`: Python Flask backend



## How to use
Start the backend, the frontend starts automatically.
```
cd backend
python app.py
```

Go to (http://localhost:8000)[http://localhost:8000]  <--- not anymore

### Prerequisites
For backend:
```
pip install -r ./backend/requirements.txt  <-- i have updated it with neo
```



## Notes
The frontend is made with Vue.js Options API and in HTML. It uses AJAX/Jquery to make polling request to the backend and update on changes.
The backend is Flask app that both serves the static files and implements the API for the different modules. It uses multithreading to run the different modules and communicate with them.

===============

PROJECT UPDATE - LEER AQUÍ :b
I have installed vue (+npm) + neo4j driver 
new port --> http://127.0.0.1:5000/data



