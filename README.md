# backend-project
This is a simple Flask-based backend that allows users to register, log in, and manage personal notes securely using JWT authentication.

Features
✅ User Registration
✅ User Login (with JWT authentication)
✅ Create Notes (only for logged-in users)
✅ View Notes
✅ Update Notes
✅ Delete Notes
✅ Secure password storage (hashed using Werkzeug)

Tech Stack
Python 3
Flask
Flask-SQLAlchemy (for database ORM)
Flask-JWT-Extended (for authentication)
SQLite (as the database)
dotenv (to manage environment variables)

API Endpoints
Method	URL	Protected	Description
POST	/register	❌	Register a new user
POST	/login	❌	Login and receive a JWT token
POST	/notes	✅	Create a new note
GET	/notes	✅	Get all your notes
PUT	/notes/<note_id>	✅	Update a note
DELETE	/notes/<note_id>	✅	Delete a note
