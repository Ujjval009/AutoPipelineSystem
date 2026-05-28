## Usage
### Option A — Start everything with one command
```bash
./start.sh
```
This launches both servers and verifies they're running.
### Option B — Start manually
#### Terminal 1 — Backend API
```bash
source venv/bin/activate
cd backend
python -m uvicorn app:app --host 0.0.0.0 --port 8000 --reload
```
#### Terminal 2 — Frontend
```bash
cd frontend
npm run dev
```
### Access
| Service | URL |
|---------|-----|
| Frontend UI | http://localhost:5173 |
| Backend API | http://localhost:8000 |
| API Docs (Swagger) | http://localhost:8000/docs |
