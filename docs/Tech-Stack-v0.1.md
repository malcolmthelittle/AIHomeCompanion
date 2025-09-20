# Tech Stack — AI Home Companion (MVP v0.1)

This document outlines the recommended technologies for the AI Home Companion MVP build. Stack decisions balance **cost (free/open-source)**, **developer availability**, and **scalability**.

---

## 📱 Frontend (Mobile App)
- **React Native** (open-source, Facebook-supported).
  - Why: One codebase for iOS & Android, strong open-source ecosystem.
- Alternatives:
  - **Flutter** (Google, also free) → excellent UI but less JavaScript synergy.

---

## ⚙️ Backend (APIs & Logic)
- **Node.js + Express** (JavaScript runtime + server framework).
  - Why: Lightweight, scalable, massive ecosystem of free libraries.
- Alternatives:
  - **Python + FastAPI** → better for heavy AI/ML but adds stack complexity.

---

## 🗄️ Database
- **PostgreSQL** (structured relational DB).
  - Why: Open-source, reliable, excellent for structured data like reminders.
- **Firebase (Free Tier)** (real-time sync + push notifications).
  - Why: Free notifications, good for chat/real-time updates.

---

## 🤖 AI Layer
- **OpenAI GPT APIs** → conversational assistant + problem diagnosis.
- **Vision APIs (OpenAI / Google Vision)** → analyze user photos.
- **Custom AI training (future phase)** → for home-specific image recognition.

---

## 🔗 Integrations (MVP Scope)
- **Zillow / Public Records APIs** → property data & valuation.
- **Thumbtack API** → local service providers.
- **Amazon / Lowe’s / Home Depot APIs** → product recommendations.
- **Pinterest API** → design inspiration.
- **Apple Home / Google Home / Amazon Alexa APIs** → smart home integration.

---

## 🌐 Hosting & DevOps
- **Supabase** → DB hosting, auth, free tier.
- **Render / Railway** → backend hosting (free tier available).
- **GitHub Actions** → CI/CD automation (free with GitHub).

---

## 🔒 Security & Auth
- **Supabase Auth** (JWT tokens) for secure login.
- **OAuth** for external services (Google, Apple, Amazon logins).

---

## 🚀 Deployment
- Mobile app: TestFlight (iOS), Google Play Internal Testing (Android).
- Backend: Deploy on Render or Railway.
- Database: Supabase-hosted Postgres.

---

## 📌 Next Steps
1. Set up GitHub repo (done).
2. Document PRD + wireframes (done).
3. Finalize tech stack (this file).
4. Create starter project (frontend + backend).
5. Begin API integrations + AI prototyping.