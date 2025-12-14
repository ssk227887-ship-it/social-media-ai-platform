# 🚀 AI-Powered Social Media Platform

**An open-source social network combining the best features of Instagram, Twitter, and Discord with AI-powered content assistance.**

## 📋 Project Overview

This project is an ambitious web platform designed for students and content creators. It combines:
- **Social networking** (follow, like, comment, share)
- **AI-powered assistant** (ChatGPT, Gemini, or Grok API integration)
- **Smart content recommendation** based on user interests
- **Real-time features** (DMs, notifications, live updates)

## ✨ Core Features (Phase 1 - MVP)

- [x] User authentication (sign up, login)
- [x] User profiles (bio, avatar, follower count)
- [ ] Text posts with images
- [ ] Like and comment system
- [ ] Follow/unfollow functionality
- [ ] Smart feed ranking
- [ ] AI post assistant (write captions, rewrite content)
- [ ] Search and discover users

## 🔮 Future Features (Phase 2+)

- Stories (24-hour posts)
- Video reels and streaming
- Direct messaging with real-time chat
- User communities and groups
- Hashtag system and trending page
- Creator monetization (subscriptions, tips)
- Ad network integration
- Dark/light mode
- Mobile app (React Native)

## 🛠️ Tech Stack

### Frontend
- **React.js** - UI framework
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling
- **Axios** - HTTP client
- **React Router** - Navigation

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web framework
- **PostgreSQL** - Main database
- **Redis** - Caching & sessions
- **Socket.io** - Real-time communication

### AI & APIs
- **OpenAI API** (ChatGPT) - Content generation
- **Google Gemini API** - Alternative AI
- **Cloudinary** - Image hosting

### DevOps & Hosting
- **GitHub** - Version control
- **Render.com** - Backend deployment
- **Vercel** - Frontend deployment
- **Railway** - Database hosting

## 📦 Project Structure

```
social-media-ai-platform/
├── frontend/                  # React application
│   ├── public/
│   ├── src/
│   │   ├── components/       # React components
│   │   ├── pages/            # Page components
│   │   ├── hooks/            # Custom React hooks
│   │   ├── services/         # API calls
│   │   └── App.js
│   └── package.json
│
├── backend/                   # Node.js/Express server
│   ├── routes/               # API endpoints
│   ├── models/               # Database models
│   ├── middleware/           # Express middleware
│   ├── controllers/          # Business logic
│   ├── services/             # Services (AI, auth, etc)
│   ├── .env.example
│   └── server.js
│
├── docs/                      # Documentation
│   ├── API.md
│   ├── SETUP.md
│   └── ARCHITECTURE.md
│
└── README.md
```

## 🚀 Quick Start

### Prerequisites
- Node.js (v16+)
- npm or yarn
- PostgreSQL
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/ssk227887-ship-it/social-media-ai-platform.git
   cd social-media-ai-platform
   ```

2. **Setup Backend**
   ```bash
   cd backend
   npm install
   cp .env.example .env
   # Configure your .env file (database, API keys)
   npm start
   ```

3. **Setup Frontend**
   ```bash
   cd ../frontend
   npm install
   npm start
   ```

4. **Open browser**
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:5000

## 📚 API Endpoints (Core)

```
AUTHENTICATION
POST   /api/auth/register       - Register new user
POST   /api/auth/login          - Login user
POST   /api/auth/logout         - Logout user

USERS
GET    /api/users/:id           - Get user profile
PUT    /api/users/:id           - Update user profile
GET    /api/users/:id/posts     - Get user's posts

POSTS
GET    /api/posts               - Get feed
POST   /api/posts               - Create post
GET    /api/posts/:id           - Get single post
PUT    /api/posts/:id           - Edit post
DELETE /api/posts/:id           - Delete post

SOCIAL
POST   /api/posts/:id/like      - Like post
POST   /api/posts/:id/unlike    - Unlike post
POST   /api/posts/:id/comment   - Comment on post
POST   /api/users/:id/follow    - Follow user
POST   /api/users/:id/unfollow  - Unfollow user

AI FEATURES
POST   /api/ai/generate-caption - Generate post caption
POST   /api/ai/rewrite          - Rewrite content
POST   /api/ai/suggestions      - Get content suggestions
```

## 🔐 Environment Variables

Create `.env` files in both backend and frontend:

**backend/.env**
```
PORT=5000
DATABASE_URL=postgresql://user:password@localhost:5432/social_media
JWT_SECRET=your_secret_key_here
OPENAI_API_KEY=sk-xxxxxxxx
GEMINI_API_KEY=your_gemini_key
CLOUDINARY_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
```

**frontend/.env**
```
REACT_APP_API_URL=http://localhost:5000/api
```

## 📖 Documentation

- [Setup Guide](./docs/SETUP.md) - Detailed installation
- [API Reference](./docs/API.md) - All endpoints
- [Architecture](./docs/ARCHITECTURE.md) - System design
- [Contributing](./CONTRIBUTING.md) - How to contribute

## 🎯 Development Roadmap

### Phase 1: MVP (Weeks 1-12)
- ✅ GitHub repo setup
- [ ] Core authentication
- [ ] Post creation & feed
- [ ] Follow system
- [ ] AI assistant integration
- [ ] Deployment

### Phase 2: Growth (Weeks 13-20)
- [ ] Stories feature
- [ ] Video support
- [ ] Direct messaging
- [ ] Notifications
- [ ] Mobile optimization

### Phase 3: Monetization (Weeks 21+)
- [ ] Creator subscriptions
- [ ] Ad network
- [ ] Premium AI features
- [ ] Analytics dashboard

## 💰 Costs

- **GitHub** - Free
- **Render.com** - Free tier / $7+/month
- **Vercel** - Free tier / $20+/month
- **PostgreSQL on Railway** - Free tier / $5+/month
- **OpenAI API** - $5 free credits + pay-as-you-go
- **Domain** - $3-12/year

**Total startup cost**: $0-30/month for MVP

## 🤝 Contributing

This project is open to contributions! Here's how to help:

1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

## 📄 License

This project is licensed under the MIT License - see [LICENSE](LICENSE) file for details.

## 📞 Support & Contact

- **Issues**: [GitHub Issues](https://github.com/ssk227887-ship-it/social-media-ai-platform/issues)
- **Email**: your.email@example.com
- **Twitter**: [@yourhandle](https://twitter.com/yourhandle)

## 🙏 Acknowledgments

- Built with inspiration from Instagram, Twitter, Discord, and LinkedIn
- AI features powered by OpenAI, Google Gemini, and Anthropic
- Hosted on Render, Vercel, and Railway
- Learning resources from FreeCodeCamp, YouTube, and official docs

---

**Made with ❤️ by a passionate developer from India 🇮🇳**

*Last updated: December 14, 2025*
