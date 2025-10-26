# lms-full-stack
A modern and scalable Full Stack Learning Management System (LMS) developed using the MERN stack. Includes user authentication, course management, educator/student dashboards, secure payments, and media uploads.

🚀 Features

    - User authentication & roles (student/educator)
    - Course CRUD, progress tracking, and purchase
    - Stripe integration for secure payments
    - Educator dashboard for content management
    - Student dashboard for enrolled courses and progress
    - Media storage on Cloudinary (images, files)
    - Responsive UI built with React
    - Modular API with authentication and error handling
    - Deployed backend (see: API Live on Vercel)

📦 Tech Stack

    - Frontend: React, Context API, Axios
    - Backend: Node.js, Express.js, MongoDB, Mongoose
    - Auth & Security: JWT, bcrypt, CORS
    - Payments: Stripe
    - Media: Cloudinary, multer
    - Other: dotenv, nodemon, Clerk (auth), Svix (webhooks)

    
📂 Project Structure
```
lms-full-stack/
├── client/                # React frontend
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   │    ├── educator/
│   │   │    └── student/
│   │   ├── context/
│   │   ├── pages/
│   │   ├── App.jsx
│   │   ├── index.css
│   │   └── main.jsx
│   └── package.json
├── server/                # Backend API
│   ├── configs/           # cloudinary.js, mongodb.js, multer.js
│   ├── controllers/
│   ├── middlewares/
│   ├── models/            # Course.js, CourseProgress.js, Purchase.js, User.js
│   ├── routes/            # courseRoute.js, educatorRoutes.js, userRoutes.js
│   ├── server.js
│   └── package.json
├── .gitignore
└── README.md

```

📋 Prerequisites
  - Node.js >= 16.x, npm >= 7.x
  - MongoDB Atlas account or local MongoDB
  - Stripe account for payments
  - Cloudinary account for media storage

⚙️ Setup & Installation
1. Clone the repository
```
git clone https://github.com/sahilk-dev/lms-full-stack.git
cd lms-full-stack
```
2. Backend
```
cd server
npm install
# Create .env with MONGO_URI, JWT_SECRET, STRIPE_SECRET, CLOUDINARY creds, etc.
npm run server
```
3. Frontend
```
cd ../client
npm install
npm start
```

🗝️ Environment Variables
server/.env example:
```
MONGO_URI=your_mongo_db_uri
JWT_SECRET=your_jwt_secret
STRIPE_SECRET=your_stripe_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

🏗️ Main Dependencies
Backend
  - express
  - mongoose
  - dotenv
  - jsonwebtoken
  - bcrypt
  - cors
  - multer
  - cloudinary
  - stripe
  - @clerk/express
  - svix
  - nodemon (dev)

Frontend
  - react
  - axios
  - react-router-dom
  - context API

🖼️ Screenshots
(To be added later)

❗ Security Best Practices
  - Never commit .env files. Ensure .gitignore includes .env, client/.env, server/.env.
  - Reset all API keys/secrets if they were ever exposed.
  - Review npm dependencies regularly.

🤝 Contributing
  - Fork the repository
  - Create your feature branch (git checkout -b feature/new-feature)
  - Commit your changes (git commit -m 'Add new feature')
  - Push to the branch (git push origin feature/new-feature)
  - Open a Pull Request

📄 License
MIT License © 2025 [Sahil Kamila]
