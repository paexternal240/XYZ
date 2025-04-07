# XYZ – Full Stack To‑Do App

A simple full‑stack application with a Flask backend and a React frontend.

---

## Prerequisites

| Tool            | Version (tested) | Notes                                          |
|-----------------|------------------|-----------------------------------------------|
| Python          | 3.8+             | Any 3.x version should work (tested on 3.11). |
| Node & npm      | Node 14+ / npm 6+| Needed for the React frontend.                |
| Git             | latest           | To clone the repository.                      |

---

## Cloning the Repository

```bash
git clone https://github.com/paexternal240/XYZ.git
cd XYZ
```

---

## Backend Setup (Flask)

1. Navigate to the **backend** folder:
   ```bash
   cd backend
   ```
2. Create and activate a virtual environment (recommended):
   ```bash
   python3 -m venv venv
   source venv/bin/activate   # on Windows use: venv\Scripts\activate
   ```
3. Install Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Flask development server:
   ```bash
   python app.py
   ```

The backend will be available at [http://localhost:5000](http://localhost:5000).

---

## Frontend Setup (React)

1. Open a new terminal window/tab and navigate to the **frontend** folder:
   ```bash
   cd frontend
   ```
2. Install JavaScript dependencies:
   ```bash
   npm install
   ```
3. Start the React development server:
   ```bash
   npm start
   ```

The frontend will run on [http://localhost:3000](http://localhost:3000) by default.

---

## Connecting Frontend & Backend

The React app expects the Flask API to be available at `http://localhost:5000`. If you changed the backend port, update the API URL inside the React code (look for calls to `fetch` or axios in `frontend/src/`).

With both servers running:

* Flask API: http://localhost:5000
* React app: http://localhost:3000

---

## Common Issues / Troubleshooting

* **`python main.py not found`** – the correct entry point is **`app.py`** in the `backend` folder.
* **CORS errors in the browser** – Flask has CORS enabled via `flask-cors` in `app.py`. Make sure you installed the dependencies with `pip install -r requirements.txt`.
* **Port already in use** – if port 3000 or 5000 is busy, either stop the other process or change the port (React: `PORT=3001 npm start`, Flask: `python app.py --port 5001`).

---

## License

MIT
