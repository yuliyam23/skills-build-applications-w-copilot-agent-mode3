# 🐙 OctoFit Tracker

A modern multi-tier fitness tracking application built with GitHub Copilot Agent Mode.

## Architecture

- **Frontend**: React 19 + Vite (Port 5173)
- **Backend**: Node.js + Express + TypeScript (Port 8000)
- **Database**: MongoDB (Port 27017)

## Quick Start

### Frontend Setup

```bash
cd octofit-tracker/frontend
npm install
npm run dev
```

The frontend will be available at `http://localhost:5173`

### Backend Setup

```bash
cd octofit-tracker/backend
npm install
cp .env.example .env
npm run dev
```

The backend will be available at `http://localhost:8000`

### Database Setup

Make sure MongoDB is running on port 27017:

```bash
# Using Docker (recommended)
docker run -d -p 27017:27017 --name mongodb mongo:latest

# Or using local MongoDB installation
mongod --port 27017
```

## Project Structure

```
octofit-tracker/
├── frontend/
│   ├── src/
│   │   ├── main.jsx
│   │   ├── App.jsx
│   │   └── App.css
│   ├── package.json
│   ├── vite.config.js
│   └── index.html
├── backend/
│   ├── src/
│   │   └── index.ts
│   ├── package.json
│   ├── tsconfig.json
│   └── .env.example
└── README.md
```

## Development

- Frontend runs with hot module replacement for instant feedback
- Backend runs with tsx watch for TypeScript development
- MongoDB serves as the persistent data layer

## Features

- React 19 with modern hooks
- TypeScript for type-safe backend development
- Express.js RESTful API
- MongoDB with Mongoose ODM
- CORS-enabled for cross-origin requests
- Environment-based configuration

## Next Steps

1. Define MongoDB schemas with Mongoose
2. Create API endpoints for fitness tracking
3. Build React components for the dashboard
4. Integrate frontend and backend communication
