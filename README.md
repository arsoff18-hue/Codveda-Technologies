# Codveda Full-Stack Development — Task Manager

A single project built to demonstrate the Codveda internship requirements across Basic, Intermediate and Advanced levels.

## Included tasks

### Level 1
- Task 1: Development environment documentation
- Task 2: REST API with Node.js + Express and CRUD endpoints
- Task 3: Frontend with HTML, CSS and Vanilla JavaScript using Fetch API

### Level 2
- Task 1: React frontend with functional components/state/API integration
- Task 2: JWT authentication, bcrypt password hashing and role-based authorization
- Task 3: MongoDB + Mongoose CRUD, validation and indexes

### Level 3
- Task 1: Full-stack React + Express + MongoDB application
- Task 2: Socket.io real-time notifications and task updates

GraphQL is not included in the core build because the internship only requires two tasks per level.

## Run locally

### 1) Backend
```bash
cd backend
copy .env.example .env
npm install
```

Open `.env` and set `MONGO_URI` and `JWT_SECRET`. Then:

```bash
npm run create-admin
npm run dev
```

API: `http://localhost:5000`

### 2) Vanilla frontend (Level 1 Task 3)
Open `frontend-vanilla/index.html` with VS Code Live Server, or any static server. Login with a registered account.

### 3) React frontend (Level 2 + Level 3)
```bash
cd frontend-react
npm install
npm run dev
```

Vite will print the local URL.

## Demo admin
Values are controlled by `.env`:
- Email: `ADMIN_EMAIL`
- Password: `ADMIN_PASSWORD`

Change the defaults before sharing the repository.

## API endpoints

- `GET /api/health`
- `POST /api/auth/register`
- `POST /api/auth/login`
- `GET /api/auth/me`
- `GET /api/tasks`
- `POST /api/tasks`
- `PUT /api/tasks/:id`
- `DELETE /api/tasks/:id`
- `GET /api/tasks/users` (admin only)

Use Postman or Thunder Client to test the endpoints.

## Submission checklist

1. Push backend + both frontend folders to GitHub.
2. Add screenshots/GIF of the working application.
3. Record a short screen video explaining the project.
4. Add the GitHub link and video link to the Codveda submission form when provided.
5. Post the project on LinkedIn and tag Codveda as required by the internship instructions.

## Suggested project explanation

“I built a Student Task Management System using React, Node.js, Express, MongoDB and Socket.io. I implemented RESTful CRUD APIs, JWT authentication with bcrypt, role-based authorization, responsive frontend integration and real-time task notifications.”
