# 🏛️ Campus Complaint Box: Next.js + Express Full-Stack Platform

> **Modern, secure, full-stack student grievance and campus governance platform with AI Assistant, Campus Heatmap Hotspots, and Community Voting System.**

---

## 🌟 Flagship Features

1. **🔥 Unique Feature #1: Interactive Campus Heatmap**
   - Live geo-spatial blueprint visualizer mapping incident density across university hostels, lecture halls, dining areas, and labs.
   - Dynamic hotspot pins with urgency pulse rings, SLA breach counters, and technician response advisories.

2. **✨ Unique Feature #2: AI Smart Complaint Assistant**
   - Natural language classification with semantic matching & confidence scoring.
   - Real-time duplicate detection shield with direct upvote redirects.
   - Automated 1-line executive summaries generated for university Deans.

3. **👍 Unique Feature #3: Community Voting System**
   - Eliminates duplicate issue backlogs by allowing hundreds of students to upvote an existing public problem.
   - Dynamic community priority escalation: complaints exceeding 15 upvotes auto-escalate to High; complaints exceeding 30 upvotes auto-escalate to Urgent.
   - Real-time Top Unresolved Concerns Leaderboard.

4. **🛡️ Comprehensive Security & Privacy**
   - Role-Based Access Control (RBAC): `STUDENT`, `STAFF`, `ADMIN`, `SUPERADMIN`.
   - Anonymous Student Identity Shielding: Personal details are cryptographically masked from staff and only verifiable in audit compliance.
   - Comprehensive audit logs recording every status change, staff assignment, and report export.

---

## 📁 Repository Structure

```
campus-complaint-box/
├── backend/                      # Production Node.js & Express API
│   ├── src/
│   │   ├── controllers/         # Auth, Complaints, AI, Staff, Analytics, Export
│   │   ├── middlewares/         # JWT, RBAC, AuditLogger, RateLimiter
│   │   ├── services/            # AI Engine, SLA Escalation Cron, Socket.io
│   │   ├── routes/              # REST Endpoints
│   │   └── server.js            # Express & WebSocket Server
│   ├── prisma/schema.prisma     # Complete PostgreSQL ORM Schema
│   └── database/schema.sql      # Raw PostgreSQL DDL with Triggers & Indexes
│
├── frontend/                     # Modern Next.js 14 App Router + Tailwind CSS
│   ├── src/
│   │   ├── app/                 # /submit, /complaints, /heatmap, /track, /admin, /analytics
│   │   ├── components/          # CampusHeatmap, AIAssistantModal, CommunityVotingCard, StatusTimeline
│   │   └── lib/                 # API Client, TypeScript Interfaces
│   ├── tailwind.config.js       # University Palette & Dark Mode Config
│   └── tsconfig.json            # Strict TypeScript Configuration
│
├── docs/                         # Architecture, Database, ER Diagram, API, Wireframes, Deployment
│   ├── ARCHITECTURE.md
│   ├── DATABASE_SCHEMA.md
│   ├── ER_DIAGRAM.md
│   ├── API_DOCUMENTATION.md
│   ├── UI_WIREFRAMES.md
│   └── DEPLOYMENT_GUIDE.md
│
└── [Standalone Web App]          # Instant zero-install browser build (index.html, submit.html, etc.)
```

---

## 🚀 How to Run

### Option A: Instant Live Browser Experience (Zero Setup)
Simply open `index.html` or `admin.html` in any web browser!
- **Home & Live Heatmap**: [index.html](file:///C:/Users/madhu_bezrb1j/.gemini/antigravity/scratch/campus-complaint-box/index.html)
- **Submit with AI Assistant**: [submit.html](file:///C:/Users/madhu_bezrb1j/.gemini/antigravity/scratch/campus-complaint-box/submit.html)
- **Community Voting Leaderboard**: [complaints.html](file:///C:/Users/madhu_bezrb1j/.gemini/antigravity/scratch/campus-complaint-box/complaints.html)
- **Track Status & Rating**: [track.html](file:///C:/Users/madhu_bezrb1j/.gemini/antigravity/scratch/campus-complaint-box/track.html)
- **Admin Console**: [admin.html](file:///C:/Users/madhu_bezrb1j/.gemini/antigravity/scratch/campus-complaint-box/admin.html) *(Username: `admin`, Password: `admin123`)*

---

### Option B: Run Full-Stack with Next.js & Express

#### 1. Backend Setup:
```bash
cd backend
npm install
npx prisma generate
npm run dev
# Server starts on port 5000 with Socket.io active
```

#### 2. Frontend Setup:
```bash
cd frontend
npm install
npm run dev
# App starts on http://localhost:3000
```

---

## ☁️ Deployment
- **Backend & Database**: Ready for 1-click deployment on [Railway.app](https://railway.app) via `railway up`.
- **Frontend**: Ready for zero-config deployment on [Vercel.com](https://vercel.com).
- Read the complete [Deployment Guide](file:///C:/Users/madhu_bezrb1j/.gemini/antigravity/scratch/campus-complaint-box/docs/DEPLOYMENT_GUIDE.md) for environment variables and production checklist.
