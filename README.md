Attendance Admin — User Guide
Overview

Attendance Admin is a web-based system for tracking student attendance in courses and sessions. Only administrators have access to the dashboard, where they can add students, courses, sessions, and record attendance.

How to Use the System

1. Login
   Open the application in your web browser (typically at http://localhost:3000 if running locally).
   Enter your administrator login and password to access the dashboard.
2. Navigating the Dashboard
   Students Tab: View, add, edit, or remove students. Use the search field to quickly find a student by name or surname.
   Courses Tab: View the list of courses. Add new courses or edit existing ones.
   Sessions Tab: View sessions (lessons) by month. Add new sessions (specify course and date), or edit/delete existing sessions.
   Attendance Tab: Select a session by month and date. Mark which students attended, and add public or private notes to each record. Save attendance for future reference.
3. PWA Features
   The system can be installed as a Progressive Web App. Click the "Install" button in your browser’s address bar or in the browser menu to add Attendance Admin to your home screen or desktop.
4. Logout
   Use the logout button in the navigation bar to end your session securely.
   Technical Requirements
   Node.js and npm installed on your machine.
   PostgreSQL database available (local or remote).
   Access credentials for an administrator account.
   Installation (for developers)

Clone the repository:

git clone https://github.com/xezo360hye/DIP392-1337.git
cd DIP392-1337

Install backend dependencies:

cd server
npm install
Configure environment variables:
Copy .env.example to .env and fill in your database connection and secret keys.

Run database migrations and seed the initial admin:

npx prisma migrate dev
npm run seed

Start the backend:

npm run dev

Install frontend dependencies and start the frontend:

cd ../client
npm install
npm start
Open in browser:
http://localhost:3000
Troubleshooting
If the backend does not start, ensure the database is running and credentials in .env are correct.
If you cannot log in, check that the admin user exists in the database.
For more help, contact the system administrator or consult project documentation.

Test Login Data:
User: admin
Pass: admin123
