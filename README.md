# Analytics and Reporting Platform

## API Documentation

**Tech Stack:** Python + FastAPI + React + Supabase

**Base URL:** `http://localhost:8000` | Deployed: `Coming soon`

**Setup:**
1. Clone repo: `git clone https://github.com/pravalikagunda/analytics-and-reporting-platform.git`
2. Backend setup:

cd backend
   pip install -r requirements.txt
   3. Create `backend/.env` file:

DATABASE_URL=your-supabase-connection-string
   SUPABASE_KEY=your-anon-key
   4. Run backend: `uvicorn main:app --reload`
5. Frontend setup:

cd frontend
   npm install
   npm run dev
   
**API Endpoints:**

### `GET /`
Root endpoint - API status  
**Response:** `{"message": "Analytics API is running"}`

### `GET /api/health`
Health check endpoint  
**Response:** `{"status": "ok", "timestamp": "2026-05-22"}`

### `GET /api/data`
Fetch analytics data  
**Response:** `{"data": [], "count": 0}`

### `POST /api/reports`
Generate a new report  
**Body:**
```json
{
  "report_type": "sales",
  "start_date": "2026-01-01",
  "end_date": "2026-01-31"
}

Response: {"report_id": "123", "status": "generated"}

Note: This is a development build. Full endpoint documentation will be updated post-deployment.

---

### **Now do this:**

1. **Delete everything** in your README editor
2. **Paste the whole thing above** 
3. Scroll down → Click **`Commit changes`**

**Done.** Step 1 = complete ✅

**Next up = Step 2: Deploy** so you get a live URL for Wexa AI. 

Is your backend code inside `backend/main.py`? If yes, we can deploy to Render in 10 mins.

**Ready to deploy now?**


