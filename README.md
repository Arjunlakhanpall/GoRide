# GoRide

A modern web platform for booking city cabs, built with React.js (frontend) and Node.js/Express (backend).

[![Live Demo](https://img.shields.io/badge/demo-live-green?style=for-the-badge)](https://arjunlakhanpall.github.io/GoRide/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

![GoRide Demo](https://github.com/user-attachments/assets/e3c20d99-1def-4237-a885-0215af8b42b5)

## Features ✨

- Real-time cab booking with fare estimation
- Driver tracking via Google Maps integration
- User/driver authentication (JWT)
- Ride history and invoices
- Multi-payment support (card, cash, e-wallet)
- Admin dashboard for managing rides
- Responsive mobile-first design

## Prerequisites 📋

- Node.js v18+
- MongoDB Atlas account (or local MongoDB)
- Google Maps API key
- npm v9+

## Installation 🛠️

### 1. Clone Repository
```bash
git clone https://github.com/arjunlakhanpall/GoRide.git
cd GoRide
```

### 2. Frontend Setup
```bash
cd frontend
npm install
```

### 3. Backend Setup
```bash
cd ../backend
npm install
```

### 4. Configuration ⚙️

#### Backend Environment (`.env`)
```plaintext
MONGODB_URI=mongodb+srv://<user>:<password>@cluster0.example.mongodb.net/goride
JWT_SECRET=your_jwt_secret_key
GOOGLE_MAPS_API_KEY=your_google_maps_key
PORT=5000
```

#### Frontend Configuration
Replace in `frontend/src/config.js`:
```javascript
export const MAPS_API_KEY = 'your_google_maps_key';
```

### 5. Running the Application ▶️

#### Start Backend Server
```bash
cd backend
npm run dev
```

#### Start Frontend
```bash
cd frontend
npm start
```

The app will be available at:
- **Frontend:** [http://localhost:3000](http://localhost:3000)
- **Backend API:** [http://localhost:5000](http://localhost:5000)

## API Endpoints 🔌

| Method | Endpoint          | Description              |
|--------|------------------|--------------------------|
| POST   | `/api/auth/signup` | User registration        |
| POST   | `/api/auth/login`  | User login              |
| POST   | `/api/rides`       | Create new ride request |
| GET    | `/api/rides`       | Get user's ride history |
| GET    | `/api/drivers`     | Get available drivers   |

## Tech Stack 💻

### Frontend
- React.js
- Tailwind CSS
- Axios (API calls)
- React Router (Navigation)
- Google Maps JavaScript API

### Backend
- Node.js
- Express.js
- MongoDB (Database)
- Mongoose (ODM)
- JWT (Authentication)

### DevOps
- GitHub Actions (CI/CD)
- Netlify (Frontend Hosting)
- Heroku (Backend Hosting)

## Deployment 🚀

### Frontend:
- Deploy to Netlify

### Backend:
- Deploy to Heroku

## Contributing 🤝

1. Fork the project
2. Create your feature branch:
```bash
git checkout -b feature/amazing-feature
```
3. Commit changes:
```bash
git commit -m 'Add some amazing feature'
```
4. Push to branch:
```bash
git push origin feature/amazing-feature
```
5. Open a Pull Request

## How to Use This README 📖
1. Replace all placeholders (e.g., `your_google_maps_key`, `<user>:<password>`)
2. Add actual screenshots to the `/screenshots` folder
3. Update API endpoints if you modify the backend
4. Include specific deployment instructions for your chosen platforms

Thank you! 🚀

