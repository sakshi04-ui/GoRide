# 🚖 GoRide – A Full-Stack Uber Clone

GoRide is a scalable, real-time cab booking platform inspired by Uber. Built using the MERN (MongoDB, Express, React, Node.js) stack, it enables seamless ride requests, driver tracking, and trip management with live location updates.

---

## 🛠️ Tech Stack

### Frontend

* React.js (with Hooks and Context API)
* Tailwind CSS (for UI styling)
* Google Maps API (for maps and location)
* Axios (for API calls)

### Backend

* Node.js + Express.js
* MongoDB with Mongoose
* Socket.io (for real-time communication)
* JWT Authentication
* RESTful APIs

---

## 📁 Folder Structure

### 🔹 Backend (`/backend`)

```
backend/
├── controllers/     → Route handlers (business logic)
├── models/          → Mongoose models
├── db/              → MongoDB connection setup
├── middleware/      → Auth, error handling, logging
├── routes/          → Express routes
├── services/        → Utility services (e.g., fare calculation, notifications)
├── socket/          → Socket.io server & event logic
├── app.js           → Express app config
├── server.js        → Server entry point
```

### 🔹 Frontend (`/frontend`)

```
frontend/
├── public/          → Static files (index.html, icons)
├── src/
│   ├── pages/       → Rider & Driver views (Home, Login, Dashboard, etc.)
│   ├── components/  → Reusable UI components (Navbar, RideCard, Map, etc.)
│   ├── context/     → Global state (UserContext, RideContext)
│   ├── assets/      → Images, logos, custom icons
│   └── App.js       → Main app setup with routing
```

---

## 🌟 Features

* ✅ Rider & Driver Registration/Login with JWT Auth
* 🚗 Book a ride and match with nearby available drivers
* 🗺️ Real-time map and location tracking using Google Maps
* 🔄 Real-time communication via Socket.io
* 💸 Ride fare calculation & ride status updates
* 🧾 Trip history and past rides
* 📱 Responsive and mobile-friendly UI

---

## 🧪 Getting Started

### Prerequisites

* Node.js (v16+)
* MongoDB (local or Atlas)
* Google Maps API Key

---

## 🚀 Local Setup

### 1. Clone the repository

```bash
git clone https://github.com/sakshi04-ui/GoRide.gitt
cd GoRide
```

### 2. Setup Backend

```bash
cd backend
npm install
```

* Create a `.env` file in `backend/` with:

```
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
GOOGLE_MAPS_API_KEY=your_google_maps_api_key
```

* Start server:

```bash
npm run dev
```

### 3. Setup Frontend

```bash
cd ../frontend
npm install
npm start
```

> The app will run at `http://localhost:3000` (frontend) and `http://localhost:5000` (backend).

---

## 🔐 Environment Variables

Your `.env` file (in `backend/`) should include:

```env
PORT=5000
MONGO_URI=mongodb+srv://your-cluster-url
JWT_SECRET=supersecretkey
GOOGLE_MAPS_API_KEY=your-api-key
```

---

## 🧠 Future Improvements

* Payment Gateway Integration (Stripe/Razorpay)
* Admin Panel for user/driver management
* Multi-language Support
* Push Notifications (Firebase)

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!
Feel free to fork the repo and submit a PR.

---

## 📄 License

This project is **open source** and available under the [MIT License](LICENSE).
