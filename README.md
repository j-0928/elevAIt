# CS Career Platform

A comprehensive platform to help students jumpstart their CS career, featuring course guidance, LeetCode practice, and career opportunities.

## Project Structure

```
cs-career-platform/
├── backend/           # FastAPI backend
│   ├── app/
│   │   ├── models/    # Database models
│   │   ├── routes/    # API routes
│   │   ├── services/  # Business logic
│   │   └── utils/     # Utility functions
│   └── requirements.txt
└── frontend/         # React frontend
    ├── src/
    │   ├── components/
    │   ├── pages/
    │   ├── services/
    │   └── utils/
    └── package.json
```

## Setup Instructions

### Backend Setup

1. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

2. Install dependencies:
   ```bash
   cd backend
   pip install -r requirements.txt
   ```

3. Create a .env file in the backend directory with the following content:
   ```
   DATABASE_URL=postgresql://postgres:postgres@localhost/cs_career_platform
   SECRET_KEY=your-secret-key-here
   ALGORITHM=HS256
   ACCESS_TOKEN_EXPIRE_MINUTES=30
   ```

4. Set up PostgreSQL database:
   - Create a database named 'cs_career_platform'
   - Update DATABASE_URL in .env if your credentials are different

5. Run the backend server:
   ```bash
   uvicorn app.main:app --reload
   ```

### Frontend Setup

1. Install dependencies:
   ```bash
   cd frontend
   npm install
   ```

2. Start the development server:
   ```bash
   npm start
   ```

## Features

- Course Roadmap
- LeetCode Practice
- Career Opportunities
- Study Groups
- Mentorship Program

## Tech Stack

### Backend
- FastAPI
- SQLAlchemy
- PostgreSQL
- Alembic (for migrations)

### Frontend
- React with TypeScript
- Material-UI
- Redux Toolkit
- React Router
- Axios 