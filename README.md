# 🌿 NurtureHub

> **Nurture Your Plants. Connect with Gardeners. Grow Together.**

A modern, intelligent plant care platform that makes gardening accessible, social, and rewarding. Connect with fellow plant enthusiasts, get AI-powered plant disease detection, and build your dream garden with our vibrant community.

![MERN Stack](https://img.shields.io/badge/Stack-MERN-green?style=flat-square&logo=mongodb&logoColor=white)
![Next.js](https://img.shields.io/badge/Frontend-Next.js-000000?style=flat-square&logo=next.js)
![Express](https://img.shields.io/badge/Backend-Express-90c53f?style=flat-square&logo=express)
![MongoDB](https://img.shields.io/badge/Database-MongoDB-13aa52?style=flat-square&logo=mongodb)

**BRAC University | CSE471 Group Project**

---

## ✨ Features

### 🪴 **Smart Plant Management**

- Create personalized plant profiles with care requirements
- Automated watering reminders and care schedules
- Track plant health metrics and growth history
- Disease identification with AI-powered image analysis

### 🤝 **Thriving Community**

- Share gardening tips and success stories
- Engage with posts through likes, comments, and shares
- Build your gardening network with other enthusiasts
- Get instant notifications about community activity

### 🛒 **Marketplace**

- Buy and sell plants, seeds, and gardening supplies
- Connect with local growers and gardeners
- Browse curated listings from the community
- Fair pricing and direct seller communication

### 📊 **Dashboard & Analytics**

- Beautiful dashboard with your garden overview
- Track multiple plants and their health status
- Gardening statistics and insights
- Weather-aware care recommendations

### 🔐 **Secure & User-Focused**

- Secure authentication with JWT tokens
- Password management and account security
- Personalized user profiles
- OAuth-ready architecture

---

## 🚀 Quick Start

### Prerequisites

- Node.js (v16+)
- MongoDB (local or Atlas)
- npm or yarn

### Installation

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd NurtureHub
   ```

2. **Setup Backend**

   ```bash
   cd nurturehub_backend
   npm install
   cp .env.example .env  # Update with your credentials
   npm run dev
   ```

   Backend runs on: `http://localhost:4000`

3. **Setup Frontend**
   ```bash
   cd nurturehub_frontend
   npm install
   cp .env.example .env  # Update with your backend URL
   npm run dev
   ```
   Frontend runs on: `http://localhost:3000`

---

## 📁 Project Structure

```
NurtureHub/
├── nurturehub_backend/          # Express.js API Server
│   ├── src/
│   │   ├── app/
│   │   │   ├── auth/            # Authentication logic
│   │   │   ├── community/       # Community posts & interactions
│   │   │   ├── market/          # Marketplace listings
│   │   │   ├── myPlant/         # Plant profiles & care tracking
│   │   │   ├── notification/    # Notifications service
│   │   │   └── userProfile/     # User management
│   │   └── server.js
│   └── package.json
│
├── nurturehub_frontend/         # Next.js Frontend
│   ├── src/
│   │   ├── app/
│   │   │   ├── (auth)           # Login & Signup pages
│   │   │   ├── dashboard/       # User dashboard
│   │   │   ├── my-plants/       # Plant management
│   │   │   ├── community/       # Social feed
│   │   │   ├── marketplace/     # Marketplace
│   │   │   ├── plant-disease-detection/ # AI detection
│   │   │   └── educational-content/    # Learning resources
│   │   └── components/          # Reusable UI components
│   └── package.json
│
└── README.md
```

---

## 🛠️ Tech Stack

### Frontend

- **Next.js 14** - React framework with SSR/SSG
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first styling
- **Axios** - HTTP client

### Backend

- **Express.js** - Minimalist web framework
- **MongoDB** - NoSQL database
- **Mongoose** - ODM for MongoDB
- **JWT** - Secure authentication
- **Nodemailer** - Email notifications
- **Bcryptjs** - Password hashing

---

## 🔑 Environment Variables

### Frontend (.env)

```env
NEXT_PUBLIC_BACKEND_URL=http://localhost:4000
NEXT_PUBLIC_API_URL=https://plant.id/api/v3/identification
NEXT_PUBLIC_API_KEY=your_plant_identification_api_key
```

### Backend (.env)

```env
PORT=4000
URI=mongodb://localhost:27017/nurturehub
JWT_SECRET=your_jwt_secret_key
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password
```

---

## 📡 API Endpoints

### Authentication

- `POST /auth/login` - User login
- `POST /auth/signup` - User registration

### Profile

- `GET /profile` - Get user profile
- `PUT /profile/update` - Update profile
- `POST /profile/changePassword` - Change password

### Plants

- `GET /myplant` - Get all user plants
- `POST /myplant` - Add new plant
- `PUT /myplant/:id` - Update plant
- `DELETE /myplant/:id` - Delete plant
- `POST /myplant/:id/water` - Log watering

### Community

- `GET /community` - Get all posts
- `POST /community` - Create post
- `POST /community/like` - Like post
- `POST /community/dislike` - Dislike post
- `POST /community/:postId/comments` - Add comment

### Marketplace

- `GET /market` - Get listings
- `POST /market` - Create listing
- `DELETE /market/:id` - Delete listing

### Notifications

- `POST /notification/sendemail` - Send email notification

---

## 🎯 Core Features Explained

### Plant Disease Detection

Uses AI-powered image analysis via plant.id API to identify plant diseases and provide treatment recommendations.

### Smart Reminders

Automatic reminders based on:

- Plant type and species
- Local weather conditions
- Seasonal care requirements
- Custom watering schedules

### Community Engagement

Users can:

- Share gardening wins and failures
- Get advice from experienced gardeners
- Collaborate on growing tips
- Build lasting gardening friendships

### Marketplace

Secure platform for buying/selling:

- Live plants
- Seeds and bulbs
- Garden tools
- Fertilizers and soil

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

## 👥 Team

BRAC University CSE471 Group Project

---

## 🐛 Issues & Support

Found a bug? Have a suggestion? Open an issue on GitHub!

---

## 🌱 Let's Grow Together!

Join our community of plant lovers and help us make gardening more accessible and fun for everyone. Happy planting! 🌿✨
