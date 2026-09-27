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

## Testing without a local MongoDB install

`test-with-memory-db.js` spins up a temporary in-memory MongoDB instance
(via `mongodb-memory-server`) and starts the API against it on port 5050 —
useful for verifying all CRUD routes without installing/configuring MongoDB
locally:

```bash
npm install
npm run test:memdb
```

Then hit `http://localhost:5050/api/interns` with GET/POST/PUT/DELETE. All
endpoints (including validation and duplicate-email conflict handling) were
verified this way.
