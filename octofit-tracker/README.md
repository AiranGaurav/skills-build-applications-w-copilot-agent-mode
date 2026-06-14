# OctoFit Tracker

A modern multi-tier fitness tracking application with React 19 frontend and Node.js/Express backend.

## Architecture

```
octofit-tracker/
├── frontend/          # React 19 + Vite (Port: 5173)
└── backend/           # Node.js + Express + TypeScript (Port: 8000)
```

## Prerequisites

- Node.js 18+ and npm/yarn
- MongoDB running on port 27017

## Frontend Setup

```bash
cd octofit-tracker/frontend
npm install
npm run dev
```

Frontend runs on: `http://localhost:5173`

## Backend Setup

```bash
cd octofit-tracker/backend
npm install
cp .env.example .env
npm run dev
```

Backend API runs on: `http://localhost:8000`

## MongoDB

Ensure MongoDB is running on port `27017`:

```bash
# Using MongoDB locally
mongod --port 27017

# Or using Docker
docker run -d -p 27017:27017 --name mongodb mongo:latest
```

## Tech Stack

### Frontend
- React 19
- Vite
- TypeScript
- CSS3

### Backend
- Node.js
- Express.js
- TypeScript
- Mongoose (MongoDB ODM)
- CORS enabled

## Scripts

### Frontend
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run lint` - Run ESLint

### Backend
- `npm run dev` - Start with hot reload (tsx watch)
- `npm run build` - Compile TypeScript
- `npm start` - Run compiled JavaScript
- `npm run lint` - Run ESLint

## Environment Variables

Create `.env` file in backend directory:

```
PORT=8000
MONGODB_URI=mongodb://localhost:27017/octofit-tracker
NODE_ENV=development
```

## Getting Started

1. **Clone and navigate to branch:**
   ```bash
   git checkout build-octofit-app
   cd octofit-tracker
   ```

2. **Install dependencies:**
   ```bash
   cd frontend && npm install && cd ../backend && npm install
   ```

3. **Start MongoDB:**
   ```bash
   mongod --port 27017
   ```

4. **Run backend:**
   ```bash
   cd backend && npm run dev
   ```

5. **Run frontend (new terminal):**
   ```bash
   cd frontend && npm run dev
   ```

6. **Access the application:**
   - Frontend: http://localhost:5173
   - Backend API: http://localhost:8000
   - MongoDB: localhost:27017
