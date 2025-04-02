# Full Stack To-Do App

A simple full-stack application with Flask backend and React frontend.

## Backend Setup

1. Navigate to the `backend` folder:
   ```bash
   cd backend
   ```

2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the server:
   ```bash
   python main.py
   ```

The backend runs on [http://localhost:5000](http://localhost:5000).

---

## Frontend Setup

1. Navigate to the `frontend` folder:
   ```bash
   cd ../frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the React app:
   ```bash
   npm start
   ```

Frontend runs on [http://localhost:3000](http://localhost:3000).

---

## Connecting Frontend and Backend

By default, the frontend fetches from the backend on port 5001. You can serve both from the backend server itself.