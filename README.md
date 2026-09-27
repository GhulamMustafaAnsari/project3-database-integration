# Project 3 — Database Integration

DecodeLabs Full Stack Industrial Training Kit (Batch 2026)

## Goal
Connect the backend with a database to store and retrieve data (Intern records).

## Key Requirements
- Design a simple database schema
- Perform basic CRUD operations
- Ensure proper data handling

## Tech
Express + MongoDB (Mongoose)

## Endpoints
| Method | Route              | Description           |
|--------|--------------------|------------------------|
| GET    | /api/interns       | List all interns       |
| GET    | /api/interns/:id   | Get one intern by id   |
| POST   | /api/interns       | Create a new intern    |
| PUT    | /api/interns/:id   | Update an intern       |
| DELETE | /api/interns/:id   | Delete an intern       |

## Setup

```bash
cp .env.example .env
npm install
npm run dev
```

Requires a running MongoDB instance (local or Atlas) at the URI set in `.env`.
