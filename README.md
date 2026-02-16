# get-social-life

**New in Hyderabad and don't know anyone?** Get Social Life puts you at a dinner table with 5 carefully matched people like you – no awkward small talk, no random meetups. Built for young tech professionals (22–30) moving to Hyderabad's startup hubs.

## Why Get Social Life?

You just landed a job at a Hyderabad tech company. You have amazing colleagues. But outside work? You're eating alone at restaurants.

Get Social Life solves this in one night. We match you with 5 people who think like you (using real personality data, not guesses), put you at a curated dinner, and let you build friendships that stick.

> "I moved to Hyderabad 3 weeks ago and felt completely isolated. One Get Social Life dinner later, I had a friend group I actually wanted to hang out with." — Priya S., Product Manager

## 🎯 How It Works

1. **Take the Personality Quiz** (5 min): Tell us about yourself — introversion/extroversion, risk tolerance, conversation style, interests, work background.
2. **We Match You** (24 hours): Our algorithm finds 5 people with compatible traits + one contrasting trait to make it interesting.
3. **Show Up & Connect** (2 hours): Dinner at a curated venue. No host, no "networking" vibe. Just real conversation.
4. **Rate & Improve** (1 min): Post-dinner feedback helps us match you better next time.

## 📊 The Matching Algorithm

We analyze **5 key dimensions** from your quiz:

- **Personality Axis**: Introvert → Extrovert
- **Risk Appetite**: Play-it-safe → Adventurous
- **Conversation Style**: Deep & focused → Broad & spontaneous
- **Work Background**: Engineering → PM/Design → Sales → Other
- **Interests**: Tech, startups, sports, arts, food, travel, etc.

We group people into tables where:
- 4 people share 3+ compatible traits (familiarity)
- 1 person brings a different perspective (growth)
- We learn from your post-dinner ratings and refine future matches

## ✨ Features

- **Personality-Matched Dinners**: Algorithm-curated tables, not random.
- **Easy Booking**: See matches, pick a dinner slot, confirm in 30 seconds.
- **Verified Attendees**: All participants are real, vetted people (no bots, no catfish).
- **Smart Schedule**: Dinners on weekends, recurring tables for regulars.
- **Safety First**: Verified profiles, ratings, and moderation.

## 🚀 Launching in Hyderabad (March 2025)

### Target Areas
- **Hitech City / Madhapur**: IT professionals, startup founders
- **Gachibowli**: Young tech workers, fresh graduates
- **Kondapur**: Mixed professionals, growth-stage companies

### Pricing
- **First Dinner**: Free (try it)
- **Recurring Dinners**: ₹299 per person (~$3.60) + venue cost (~₹500–800 per head)
- **Group Subscriptions**: ₹2,499/month for unlimited dinners

### Get on the Waitlist
[Join the Hyderabad launch waitlist](https://link.com) — First 100 get free dinners.

## 🛠️ Tech Stack

### Frontend
- **React.js** with TypeScript
- **Vite** for fast builds
- **Tailwind CSS** for UI
- **Axios** for API calls

### Backend
- **Node.js** with Express
- **MongoDB** for user profiles & matching data
- **JWT** for authentication
- **Socket.io** for real-time notifications

### AI/ML
- **Python** (Flask) for matching algorithm
- **scikit-learn** for similarity scoring
- **Feedback loop** to improve recommendations

### Deployment
- **AWS EC2** for backend
- **Vercel** for frontend
- **MongoDB Atlas** for database
- **Redis** for caching

## 📖 Setup & Installation

### Prerequisites
- Node.js v18+
- Python 3.9+
- MongoDB running locally or Atlas connection string

### Quick Start

```bash
# Clone the repo
git clone https://github.com/ramji3030/get-social-life.git
cd get-social-life

# Install dependencies
# Frontend
cd client
npm install

# Backend
cd ../server
npm install

# Python matching engine
cd ../ml_engine
pip install -r requirements.txt

# Setup environment variables
cp .env.example .env
# Edit .env with your MongoDB URI, JWT secret, etc.

# Run development server
cd ../server
npm run dev

# In another terminal, start frontend
cd ../client
npm run dev

# In another terminal, start Python matching service
cd ../ml_engine
python app.py
```

## 📝 Configuration

Create a `.env` file in the `server` directory:

```env
MONGODB_URI=mongodb+srv://your-username:your-password@cluster.mongodb.net/get-social-life
JWT_SECRET=your-secret-key-here
PORT=5000
FRONTEND_URL=http://localhost:5173
ML_ENGINE_URL=http://localhost:5001
```

## 🗂️ Project Structure

```
get-social-life/
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/    # UI components
│   │   ├── pages/         # Page routes
│   │   └── hooks/         # Custom React hooks
│   └── package.json
├── server/                 # Node.js/Express backend
│   ├── routes/            # API routes
│   ├── models/            # Database schemas
│   ├── controllers/        # Request handlers
│   └── package.json
├── ml_engine/              # Python matching algorithm
│   ├── models/            # ML models & logic
│   ├── utils/             # Helper functions
│   └── requirements.txt
└── README.md
```

## 🧠 The Matching Logic (Under the Hood)

Our algorithm uses **cosine similarity** to match personality profiles:

1. **Vectorize Profiles**: Convert quiz answers to numerical vectors
2. **Calculate Similarity Score**: 0 = opposite, 1 = identical
3. **Group into Tables**: Select 5 people with avg similarity 0.65–0.80
4. **Iterative Learning**: Post-dinner ratings feedback into next matches

Example: Two people both answer "extroverted" + "tech background" = high similarity. Add one "introverted designer" for diversity.

## 🔒 Security

- **JWT Authentication**: Secure token-based login
- **Profile Verification**: Email + phone verification before dining
- **Rate Limiting**: Prevent spam and abuse
- **Data Privacy**: User data is encrypted and never shared without consent

## 📈 Roadmap

- [x] Core matching algorithm (MVP)
- [x] Basic web app
- [ ] Launch in Hyderabad (March 2025)
- [ ] Expand to Bangalore, Mumbai (Q2 2025)
- [ ] Mobile app (iOS/Android) (Q3 2025)
- [ ] Payment integration (Razorpay, Stripe)
- [ ] AI chatbot for post-dinner networking tips
- [ ] Sponsor partnerships (restaurants, brands)

## 💰 For Investors

Get Social Life is a high-growth social platform solving the loneliness problem for 300M+ young professionals in India's cities. We're launching in Hyderabad with a proven unit economics model and immediate path to scale.

### Why Invest?

- **Massive Market**: 100M+ professionals aged 22-35 in Indian metros; growing at 15% annually
- **Network Effects**: Personality matching creates viral retention; users become super-connectors
- **Multiple Revenue Streams**: B2C (dinners), B2B2C (employer partnerships), premium features, venue commissions
- **Founder Traction**: Core algorithm built, MVP tested with early users
- **Proven Unit Economics**: First 100 dinners cost ₹2,500; retail at ₹800–1,200 per head

### Investment Ask

**Seed Round: $250K–$500K**
- Launch in Hyderabad (100 dinners/month within 90 days)
- Expand to Bangalore + Pune (Q2 2025)
- Build mobile app (Q3 2025)
- Hire founding team (1–2 engineers, 1 operations lead)

### Contact Us for Investor Deck

📧 **Email**: [investors@getsociallife.in](mailto:investors@getsociallife.in)  
🔗 **LinkedIn**: [Ramji Bharath](https://linkedin.com/in/ramji-bharath)  
💬 **Telegram**: @ramji3030  
🤝 **Let's talk growth**: Reply to this repo or book a 20-min call

---



## 💬 Feedback & Support

Have questions or bugs? Open an issue on GitHub or email us at [hello@getsociallife.in](mailto:hello@getsociallife.in).

## 📄 License

MIT License — See LICENSE.md for details.

---

### For Developers: Key Documentation

- [**Setup Guide**](./docs/SETUP.md) — Environment & local dev setup
- [**API Reference**](./docs/API.md) — Backend endpoints
- [**Deployment**](./docs/DEPLOYMENT.md) — AWS/Vercel deployment
- [**Market Strategy**](./HYDERABAD_MARKET_STRATEGY.md) — Go-to-market plan

---

**Made with ❤️ to help people build real friendships in a new city.**
