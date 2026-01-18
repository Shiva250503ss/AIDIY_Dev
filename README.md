<div align="center">

# 🧒💰 AIDIY - AI-Powered Financial Literacy Platform

### *Teaching Kids Smart Money Habits Through AI & Gamification*

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Flask](https://img.shields.io/badge/Flask-2.0+-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org)
[![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://mongodb.com)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4o-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com)

<br/>

[Features](#-key-features) • [Architecture](#-system-architecture) • [Tech Stack](#-technology-stack) • [Installation](#-quick-start) • [API](#-api-documentation)

---

</div>

## 📋 Project Overview

**AIDIY** is an end-to-end **AI-powered EdTech platform** designed to revolutionize how children learn financial literacy. By combining **machine learning**, **natural language processing**, and **gamification strategies**, this platform delivers personalized learning experiences that adapt to each child's unique needs.

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                         AIDIY PLATFORM ECOSYSTEM                            │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│    👨‍👩‍👧‍👦 PARENTS                    🤖 AI ENGINE                 👶 CHILDREN    │
│    ┌─────────────┐              ┌─────────────┐              ┌───────────┐  │
│    │ Dashboard   │◄────────────►│ GPT-4o NLP  │◄────────────►│ Gamified  │  │
│    │ Analytics   │              │ Voice AI    │              │ Learning  │  │
│    │ Task Mgmt   │              │ Insights    │              │ Rewards   │  │
│    └─────────────┘              └─────────────┘              └───────────┘  │
│           │                           │                           │         │
│           └───────────────────────────┼───────────────────────────┘         │
│                                       ▼                                     │
│                          ┌─────────────────────┐                            │
│                          │   📊 DATA LAYER     │                            │
│                          │  MongoDB + Redis    │                            │
│                          │  Real-time Sync     │                            │
│                          └─────────────────────┘                            │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 🎯 Key Features

<table>
<tr>
<td width="50%">

### 🔬 AI & Machine Learning
- **GPT-4o Integration** - Context-aware conversational AI
- **Speech-to-Text** - Real-time voice processing
- **Personalized Recommendations** - Adaptive learning paths
- **Sentiment Analysis** - Understanding user engagement

</td>
<td width="50%">

### 📊 Data Analytics & Insights
- **Progress Tracking** - Real-time learning metrics
- **Behavioral Analytics** - User interaction patterns
- **Performance Dashboards** - Visual data storytelling
- **Assessment Scoring** - Multi-dimensional evaluation

</td>
</tr>
<tr>
<td width="50%">

### 🏗️ Data Engineering
- **RESTful API Design** - Scalable endpoint architecture
- **MongoDB Aggregation** - Complex data pipelines
- **JWT Authentication** - Secure token management
- **Real-time Data Sync** - Cross-platform consistency

</td>
<td width="50%">

### 🎮 User Experience
- **Gamification Engine** - Points, badges, rewards
- **Multi-child Profiles** - Family management system
- **Responsive Design** - Mobile-first approach
- **Animated AI Avatar** - Engaging interactions

</td>
</tr>
</table>

---

## 🏛️ System Architecture

```
┌────────────────────────────────────────────────────────────────────────────────┐
│                              CLIENT LAYER (React 18)                           │
├────────────────────────────────────────────────────────────────────────────────┤
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐       │
│  │   HomePage   │  │  Dashboard   │  │  Assessment  │  │   AI Chat    │       │
│  │   Component  │  │  Analytics   │  │    Quiz      │  │   Interface  │       │
│  └──────┬───────┘  └──────┬───────┘  └──────┬───────┘  └──────┬───────┘       │
│         │                 │                 │                 │                │
│         └─────────────────┴─────────────────┴─────────────────┘                │
│                                    │                                           │
│                          ┌─────────▼─────────┐                                 │
│                          │   Redux Toolkit   │                                 │
│                          │   State Manager   │                                 │
│                          └─────────┬─────────┘                                 │
└────────────────────────────────────┼───────────────────────────────────────────┘
                                     │ HTTPS/REST
┌────────────────────────────────────┼───────────────────────────────────────────┐
│                              API GATEWAY LAYER                                 │
├────────────────────────────────────┼───────────────────────────────────────────┤
│                          ┌─────────▼─────────┐                                 │
│                          │   Flask Server    │                                 │
│                          │   (Python 3.8+)   │                                 │
│                          └─────────┬─────────┘                                 │
│         ┌──────────────────────────┼──────────────────────────┐                │
│         │                          │                          │                │
│  ┌──────▼──────┐           ┌───────▼───────┐          ┌───────▼───────┐       │
│  │    Auth     │           │   User Mgmt   │          │   AI Service  │       │
│  │  /auth/*    │           │   /api/users  │          │   /api/ai/*   │       │
│  │  JWT+OAuth  │           │   CRUD Ops    │          │   NLP Engine  │       │
│  └──────┬──────┘           └───────┬───────┘          └───────┬───────┘       │
└─────────┼──────────────────────────┼──────────────────────────┼────────────────┘
          │                          │                          │
┌─────────┼──────────────────────────┼──────────────────────────┼────────────────┐
│         │                   DATA LAYER                        │                │
├─────────┼──────────────────────────┼──────────────────────────┼────────────────┤
│  ┌──────▼──────┐           ┌───────▼───────┐          ┌───────▼───────┐       │
│  │   MongoDB   │           │   User Data   │          │   OpenAI API  │       │
│  │   Atlas     │◄─────────►│   Collections │          │   GPT-4o      │       │
│  │   Cluster   │           │   Indexes     │          │   Whisper     │       │
│  └─────────────┘           └───────────────┘          └───────────────┘       │
└────────────────────────────────────────────────────────────────────────────────┘
```

---

## 💻 Technology Stack

<div align="center">

### Backend & Data Engineering
| Technology | Purpose | Skill Category |
|:----------:|:--------|:---------------|
| ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) | Core backend logic, API development | **Data Engineering** |
| ![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white) | RESTful API framework | **Backend Development** |
| ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) | NoSQL database, aggregation pipelines | **Data Engineering** |
| ![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white) | Secure authentication tokens | **Security** |

### AI & Machine Learning
| Technology | Purpose | Skill Category |
|:----------:|:--------|:---------------|
| ![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white) | GPT-4o for conversational AI | **AI Engineering** |
| ![NLP](https://img.shields.io/badge/NLP-FF6F00?style=flat-square&logo=tensorflow&logoColor=white) | Natural Language Processing | **Data Science** |
| ![Speech](https://img.shields.io/badge/Whisper-74aa9c?style=flat-square&logo=openai&logoColor=white) | Speech-to-text processing | **AI Engineering** |

### Frontend & Visualization
| Technology | Purpose | Skill Category |
|:----------:|:--------|:---------------|
| ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) | Component-based UI | **Full Stack** |
| ![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat-square&logo=redux&logoColor=white) | State management | **Full Stack** |
| ![TailwindCSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white) | Responsive styling | **UI/UX** |

</div>

---

## 📈 Data Pipeline & Analytics

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                          DATA FLOW ARCHITECTURE                              │
└─────────────────────────────────────────────────────────────────────────────┘

  USER INTERACTIONS          DATA PROCESSING           INSIGHTS GENERATION
  ─────────────────         ─────────────────         ────────────────────
        │                          │                          │
        ▼                          ▼                          ▼
  ┌───────────┐             ┌───────────┐             ┌───────────────┐
  │  Events   │────────────►│  ETL      │────────────►│  Aggregated   │
  │  Capture  │             │  Pipeline │             │  Metrics      │
  └───────────┘             └───────────┘             └───────────────┘
        │                          │                          │
        ▼                          ▼                          ▼
  ┌───────────┐             ┌───────────┐             ┌───────────────┐
  │  Quiz     │────────────►│  Score    │────────────►│  Learning     │
  │  Answers  │             │  Compute  │             │  Analytics    │
  └───────────┘             └───────────┘             └───────────────┘
        │                          │                          │
        ▼                          ▼                          ▼
  ┌───────────┐             ┌───────────┐             ┌───────────────┐
  │  Voice    │────────────►│  Speech   │────────────►│  Sentiment    │
  │  Input    │             │  Analysis │             │  Insights     │
  └───────────┘             └───────────┘             └───────────────┘
```

### Assessment Analytics Engine

The platform evaluates children across **6 key financial literacy dimensions**:

| Dimension | Metrics Tracked | Analysis Type |
|-----------|-----------------|---------------|
| 💵 Money Recognition | Accuracy, Response Time | Quantitative |
| 🏦 Saving Habits | Frequency, Consistency | Behavioral |
| 💼 Understanding Earning | Concept Grasp | Qualitative |
| 🛒 Wants vs Needs | Decision Patterns | Classification |
| 🎯 Purchasing Decisions | Risk Assessment | Predictive |
| 📊 Financial Responsibility | Progress Tracking | Longitudinal |

---

## 🚀 Quick Start

### Prerequisites

```bash
Python 3.8+  │  Node.js 14+  │  MongoDB  │  OpenAI API Key
```

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/AIDIY-Dev.git && cd AIDIY-Dev

# 2. Backend setup
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt

# 3. Frontend setup
cd client && npm install

# 4. Configure environment
cp .env.example .env
# Edit .env with your credentials
```

### Environment Variables

```env
# Database
MONGODB_URI=mongodb+srv://your-cluster-url

# Authentication
JWT_SECRET=your-secure-secret-key

# AI Services
OPENAI_API_KEY=sk-your-api-key

# Email (Optional)
EMAIL_HOST=smtp.gmail.com
EMAIL_USER=your-email@gmail.com
```

### Launch

```bash
# Terminal 1: Start Backend (Port 5500)
python app.py

# Terminal 2: Start Frontend (Port 3000)
cd client && npm start
```

---

## 📡 API Documentation

### Authentication Endpoints

| Method | Endpoint | Description | Auth |
|--------|----------|-------------|------|
| `POST` | `/auth/register` | User registration with OTP | ❌ |
| `POST` | `/auth/verify-otp` | Email verification | ❌ |
| `POST` | `/auth/login` | JWT token generation | ❌ |
| `POST` | `/auth/google` | OAuth 2.0 authentication | ❌ |
| `POST` | `/api/auth/logout` | Session termination | ✅ |

### User Management

| Method | Endpoint | Description | Auth |
|--------|----------|-------------|------|
| `GET` | `/api/users/profile` | Fetch user data | ✅ |
| `PUT` | `/api/users/profile` | Update profile | ✅ |
| `GET` | `/api/users/children` | List children profiles | ✅ |
| `POST` | `/api/users/children` | Create child profile | ✅ |

### AI Services

| Method | Endpoint | Description | Auth |
|--------|----------|-------------|------|
| `POST` | `/api/ai/chat` | GPT-4o conversation | ✅ |
| `POST` | `/api/ai/speech-to-text` | Whisper transcription | ✅ |

---

## 📁 Project Structure

```
AIDIY-Dev/
│
├── 📊 app.py                    # Flask application entry point
├── 📋 requirements.txt          # Python dependencies
├── 🔐 .env                      # Environment configuration
│
├── 🖥️ client/                   # React Frontend
│   ├── src/
│   │   ├── components/          # UI Components
│   │   │   ├── HomePage.jsx
│   │   │   ├── ParentDashboard.jsx
│   │   │   ├── AssessmentQuiz.jsx
│   │   │   └── AIAvatar.jsx
│   │   ├── store/               # Redux State Management
│   │   └── App.js
│   └── package.json
│
├── 🔧 server/                   # API Routes & Services
│   ├── routes/
│   ├── models/
│   └── services/
│
└── 📖 README.md
```

---

## 🔒 Security Implementation

| Feature | Implementation | Purpose |
|---------|----------------|---------|
| **Password Hashing** | bcrypt with salt rounds | Secure credential storage |
| **Token Management** | JWT with expiration | Stateless authentication |
| **CORS Policy** | Whitelist configuration | Cross-origin protection |
| **Input Validation** | Server-side sanitization | Injection prevention |
| **OAuth 2.0** | Google authentication | Third-party auth security |

---

## 🧠 Skills Demonstrated

<div align="center">

| Data Analyst | Data Scientist | Data Engineer | AI Engineer |
|:------------:|:--------------:|:-------------:|:-----------:|
| Dashboard Design | ML Integration | API Development | GPT-4o Integration |
| KPI Tracking | NLP Processing | Database Design | Speech-to-Text |
| Data Visualization | Predictive Models | ETL Pipelines | Prompt Engineering |
| User Analytics | Feature Engineering | Data Modeling | Conversational AI |
| Progress Metrics | Sentiment Analysis | Query Optimization | Voice Processing |

</div>

---

## 🔮 Future Enhancements

- [ ] **Real-time Analytics Dashboard** - Apache Kafka integration
- [ ] **ML Recommendation Engine** - TensorFlow/PyTorch models
- [ ] **Data Warehouse** - AWS Redshift/BigQuery integration
- [ ] **A/B Testing Framework** - Statistical significance testing
- [ ] **Advanced NLP** - Custom fine-tuned models

---

<div align="center">

### 🤝 Let's Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin)](https://linkedin.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-000000?style=for-the-badge&logo=vercel)](https://portfolio.com)
[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail)](mailto:your@email.com)

---

*Built with passion for education and technology*

**⭐ Star this repo if you found it interesting!**

</div>
