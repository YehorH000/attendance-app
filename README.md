# Attendance Admin

## Overview

Attendance Admin is a web-based system for managing student attendance across courses and sessions. Administrators can manage students, courses, sessions, and attendance records through a secure dashboard.

---

## Features

- Secure administrator authentication
- Student management (create, edit, delete, search)
- Course management
- Session management with monthly filtering
- Attendance tracking with public and private notes
- Responsive interface for desktop and mobile devices
- Progressive Web App (PWA) support

---

## Technologies

### Frontend

- React
- TypeScript
- Material UI
- Axios

### Backend

- Node.js
- Express.js
- Prisma ORM

### Database

- PostgreSQL

---

## Installation

### Clone the repository

```bash
git clone https://github.com/xezo360hye/DIP392-1337.git
cd DIP392-1337
```

### Backend

Install dependencies:

```bash
cd server
npm install
```

Create a `.env` file and configure your database connection.

Run database migrations and generate Prisma Client:

```bash
npx prisma migrate dev
npx prisma generate
```

Create the administrator account:

```bash
npm run seed
```

Start the backend:

```bash
npm run dev
```

### Frontend

Install dependencies:

```bash
cd ../client
npm install
npm start
```

The application will be available at:

```
http://localhost:3000
```

---

## User Guide

### Login

Sign in using an administrator account.

Default credentials:

- **Login:** `admin`
- **Password:** `admin123`

### Dashboard

#### Students

- Add, edit and delete students
- Search students by name or surname
- View attendance history

#### Courses

- Create, edit and delete courses

#### Sessions

- Create, edit and delete sessions
- Filter sessions by month

#### Attendance

- Select a month and session
- Mark attendance
- Add public and private notes
- Save attendance records

### Progressive Web App

The application can be installed as a Progressive Web App (PWA) using your browser's **Install App** option.

### Logout

Use the logout button to end the session securely.

---

## Troubleshooting

- Make sure PostgreSQL is running.
- Verify the `.env` configuration.
- Run `npx prisma generate` if Prisma Client is missing.
- Run `npm run seed` if the administrator account does not exist.
