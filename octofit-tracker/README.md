# OctoFit Tracker

A modern multi-tier fitness tracking application built with GitHub Copilot Agent Mode.

## Architecture

- **Frontend**: React 19 + Vite (Port 5173)
- **Backend**: Node.js + Express + TypeScript (Port 8000)
- **Database**: MongoDB (Port 27017)

## Setup Instructions

### Prerequisites

- Node.js 18+
- MongoDB running locally or accessible
- npm or yarn

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

### MongoDB Setup

Ensure MongoDB is running on `localhost:27017` or update the `MONGODB_URI` in `.env`

## Available Endpoints

- `GET /health` - Health check endpoint
- More endpoints coming soon...

## Development

- Frontend: Run `npm run dev` in the frontend directory
- Backend: Run `npm run dev` in the backend directory

## Building for Production

### Frontend
```bash
npm run build
```

### Backend
```bash
npm run build
npm start
```

## Project Structure

```
octofit-tracker/
├── frontend/
│   ├── src/
│   ├── package.json
│   ├── vite.config.js
│   └── index.html
└── backend/
    ├── src/
    ├── package.json
    ├── tsconfig.json
    └── .env.example
```
