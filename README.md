Prescripto 🏥
A full-stack doctor appointment booking web application built with the MERN stack. Patients can browse doctors, book appointments, and manage their profiles. Admins can manage doctors and appointments through a dedicated admin panel.

🌐 Live Demo
Frontend: https://prescripto-sepia-five.vercel.app
AdminPanel: https://prescripto-2a5y.vercel.app
Backend API: https://prescripto-backend-0j94.onrender.com

✨ Features
👤 Patient (Frontend)

Register and log in securely with JWT authentication
Browse all available doctors filtered by speciality
Book, view, and cancel appointments
Update profile with photo, phone number, address, date of birth, and gender
Image uploads handled via Cloudinary

🛡 Admin Panel

Secure admin login
Add new doctors with full details and profile image
View and manage all appointments across all patients
Cancel appointments from the admin dashboard
Dashboard overview with total doctors, patients, and appointments count

⚙️ Backend

RESTful API built with Express.js
JWT-based authentication for both users and admins
MongoDB database via Mongoose
Cloudinary integration for image storage
Multer middleware for handling file uploads


🧰 Tech Stack
Frontend & Admin
TechnologyPurposeReact.js (Vite)UI frameworkTailwind CSSStylingAxiosAPI requestsReact Router DOMClient-side routing
Backend
TechnologyPurposeNode.jsRuntimeExpress.jsServer frameworkMongoDB + MongooseDatabaseJWTAuthenticationBcryptPassword hashingCloudinaryImage hostingMulterFile upload handlingValidatorInput validation

📁 Project Structure
Prescripto/
├── frontend/               # Patient-facing React app
├── admin/                  # Admin panel React app
└── backend/                # Express REST API
    ├── controllers/        # Route logic
    ├── models/             # Mongoose schemas
    ├── routes/             # API routes
    ├── middleware/         # Auth & upload middleware
    └── config/             # DB & Cloudinary config

🚀 Running Locally
Prerequisites

Node.js installed
MongoDB Atlas account
Cloudinary account

1. Clone the repository
bashgit clone https://github.com/Abhiraj121212/Prescripto.git
cd Prescripto
2. Setup Backend
bashcd backend
npm install
Create a .env file inside the backend folder:
envMONGODB_URI=your_mongodb_atlas_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET_KEY=your_cloudinary_secret_key
ADMIN_EMAIL=your_admin_email
ADMIN_PASSWORD=your_admin_password
CURRENCY=INR
Start the backend server:
bashnode server.js
3. Setup Frontend
bashcd frontend
npm install
Create a .env file inside the frontend folder:
envVITE_BACKEND_URL=http://localhost:4000
Start the frontend:
bashnpm run dev
4. Setup Admin
bashcd admin
npm install
Create a .env file inside the admin folder:
envVITE_BACKEND_URL=http://localhost:4000
Start the admin panel:
bashnpm run dev

☁️ Deployment
This project is deployed using the following services:
ServicePurposeVercelFrontend & Admin panel hostingRenderBackend API hostingMongoDB AtlasCloud databaseCloudinaryImage storage


📄 License
This project is open source and available under the MIT License.
