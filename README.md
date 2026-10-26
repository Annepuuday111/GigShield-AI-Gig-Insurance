<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF6B6B,35:FFA94D,70:4DABF7,100:845EF7&height=200&section=header&text=GigShield&fontSize=44&fontColor=ffffff&fontAlignY=36&animation=fadeIn&desc=AI-powered%20parametric%20insurance%20for%20gig%20delivery%20workers&descSize=16&descAlignY=58" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=845EF7&center=true&vCenter=true&width=700&lines=Weekly+cover+for+delivery+partners;AI+risk-based+premium+pricing;Auto-filed+claims+on+weather+triggers;Fraud+scoring+%2B+instant+wallet+payouts" alt="Typing SVG"/>

<br/>

<img src="https://img.shields.io/badge/React%2018-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite"/>
<img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS"/>
<img src="https://img.shields.io/badge/Java%2017-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java"/>
<img src="https://img.shields.io/badge/Spring%20Boot%203-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" alt="Spring Boot"/>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" alt="Firebase"/>
<img src="https://img.shields.io/badge/Razorpay-0C2451?style=for-the-badge&logo=razorpay&logoColor=white" alt="Razorpay"/>

<br/>

<img src="https://img.shields.io/badge/Status-Active-20C997?style=for-the-badge" alt="Status"/>
<img src="https://img.shields.io/github/stars/Annepuuday111/GigShield-AI-Gig-Insurance?style=for-the-badge&color=845EF7" alt="Stars"/>
<img src="https://img.shields.io/github/last-commit/Annepuuday111/GigShield-AI-Gig-Insurance?style=for-the-badge&color=4DABF7" alt="Last Commit"/>
<img src="https://img.shields.io/github/repo-size/Annepuuday111/GigShield-AI-Gig-Insurance?style=for-the-badge&color=FF6B6B" alt="Repo Size"/>

<br/><br/>

[About](#-about) • [Features](#-features) • [Tech Stack](#️-tech-stack) • [Architecture](#️-architecture) • [Getting Started](#-getting-started) • [Screenshots](#-screenshots) • [Author](#-author)

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 📖 About

**GigShield** is a parametric micro-insurance platform for India's gig delivery partners (Zomato, Swiggy, Amazon, Flipkart, Zepto, Dunzo and more). Workers buy a **weekly plan**, and a scheduled job checks each active policy against weather and disruption triggers. When a trigger fires, a claim is filed automatically; claims are verified with a Python AI service (including fraud scoring) and approved payouts land in the worker's in-app wallet.

The system is split into three services:

- **`frontend/`** – React + Vite + Tailwind web app for workers and admins
- **`backend/`** – Spring Boot 3 REST API (JWT security, MySQL, scheduler, email OTP, Razorpay)
- **`ai-model/`** – FastAPI service for premium pricing, risk scoring, parametric trigger checks and fraud detection

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## ✨ Features

### 🛵 For delivery workers
- 📝 **Sign up with email OTP** or **Google sign-in** (Firebase Auth), with platform and location (state / district) captured at registration
- 🛡️ **Weekly insurance plans** with AI-recommended plan and risk-adjusted premium
- 💳 **Payments** via Razorpay checkout or UPI / other methods recorded for admin approval
- 🤖 **Automatic parametric claims** – an hourly job checks active subscriptions against plan triggers (rainfall, heat, wind, AQI, etc.)
- 🧾 **Manual situation requests** – file a claim that is AI-verified and auto-approved or flagged
- 👛 **Wallet** credited on approved claims, with payment history
- 📊 **AI insights & reports** – risk score, weather snapshot, triggers and activity charts
- 🔔 **Notifications** and 💬 **support chat** with the admin team
- 🎨 Dashboard themed to the worker's delivery platform

### 👑 For admins
- Manage users, plans (premium, coverage, parametric triggers) and partner platforms
- Review, approve or reject claims and payments
- Insurance-fund wallet overview and weather report
- Answer user support queries

### 🧠 AI service (`ai-model/main.py`)
- Risk score from platform, state, season and tenure → premium multiplier
- Parametric trigger evaluation including custom per-plan triggers
- Rule-based fraud scoring (duplicate window, missing subscription, location mismatch, weather corroboration, …)
- Deterministic mock weather per location/day for repeatable demos

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 🛠️ Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=react,vite,tailwind,java,spring,mysql,python,fastapi,firebase,docker&theme=light" alt="Tech icons"/>

</div>

| Layer | Technology |
| :--- | :--- |
| **Frontend** | ![React](https://img.shields.io/badge/React%2018-61DAFB?style=for-the-badge&logo=react&logoColor=black) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white) ![Tailwind](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white) ![React Router](https://img.shields.io/badge/React%20Router-CA4245?style=for-the-badge&logo=reactrouter&logoColor=white) |
| **Backend** | ![Java](https://img.shields.io/badge/Java%2017-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring%20Boot%203.2-6DB33F?style=for-the-badge&logo=springboot&logoColor=white) ![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white) ![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white) |
| **Database** | ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white) ![Hibernate](https://img.shields.io/badge/Spring%20Data%20JPA-59666C?style=for-the-badge&logo=hibernate&logoColor=white) |
| **AI Service** | ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white) ![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=for-the-badge&logo=pydantic&logoColor=white) |
| **Auth & Integrations** | ![Firebase](https://img.shields.io/badge/Firebase%20Auth-FFCA28?style=for-the-badge&logo=firebase&logoColor=black) ![Razorpay](https://img.shields.io/badge/Razorpay-0C2451?style=for-the-badge&logo=razorpay&logoColor=white) ![Gmail SMTP](https://img.shields.io/badge/SMTP%20OTP-EA4335?style=for-the-badge&logo=gmail&logoColor=white) |
| **DevOps** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white) ![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white) |

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 🏗️ Architecture

```text
 React + Vite (frontend, :5173)
        │  REST + JWT   (VITE_API_URL)
        ▼
 Spring Boot API (backend, :4000) ──── MySQL (JPA / Hibernate)
        │   ├── AutoClaimService  @Scheduled hourly: check active subscriptions
        │   │                     @Scheduled 30 min: re-verify pending claims
        │   ├── EmailService      OTP & notification emails (SMTP)
        │   └── RazorpayService   orders & signature verification
        │  HTTP (AI_SERVICE_URL)
        ▼
 FastAPI AI service (ai-model, :8000)
        /ai/premium · /ai/risk · /ai/fraud/detect · /ai/parametric/check
        /ai/weather · /ai/dashboard · /ai/plans/recommend · /ai/fraud/stats
```

**Claim flow:** worker buys a 7-day subscription → hourly scheduler calls `/ai/parametric/check` for the worker's location and plan triggers → if a trigger fires, a claim is filed automatically and the worker is notified. Manually filed situation requests are scored via `/ai/fraud/detect` and approved or flagged for admin review. Approved claims are credited to the worker's wallet from the insurance fund. Plans expire automatically after 7 days.

### 📂 Project Structure

```text
GigShield-AI-Gig-Insurance/
├── frontend/                     # React + Vite + Tailwind
│   ├── src/
│   │   ├── pages/                # Landing, Login, Register, Dashboard, Plans, Payment,
│   │   │                         # Claims, Insights, Reports, Notifications, ChatSupport,
│   │   │                         # Profile, AdminDashboard
│   │   ├── components/           # Navbar, Sidebar, BottomNav, cards, ProtectedRoute ...
│   │   ├── layouts/MainLayout.jsx
│   │   ├── api.js                # REST client (VITE_API_URL)
│   │   └── firebase.js           # Google sign-in
│   └── package.json
├── backend/                      # Spring Boot 3 (Java 17)
│   ├── src/main/java/com/example/aiinsurance/
│   │   ├── controller/           # Auth, Plan, Subscription, ClaimRequest, PaymentGateway,
│   │   │                         # Admin, AI, Notification, Partner, Query ...
│   │   ├── model/                # User, Admin, Plan, Subscription, ClaimRequest, Payment,
│   │   │                         # Notification, Partner, Query
│   │   ├── repository/
│   │   ├── security/             # JwtUtil, JwtAuthenticationFilter, SecurityConfig
│   │   └── service/              # AutoClaimService, ClaimService, AIService, RazorpayService ...
│   ├── src/main/resources/application.properties
│   ├── Dockerfile
│   └── pom.xml
├── ai-model/                     # FastAPI AI service
│   ├── main.py
│   ├── requirements.txt
│   └── Dockerfile
├── docs/                         # architecture.md, workflow.md
├── assets/                       # Screenshots & platform banners
├── start.sh                      # One-command startup (macOS / Linux)
└── start.bat                     # One-command startup (Windows)
```

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 🚀 Getting Started

### Prerequisites

- Java 17+ and Maven
- Node.js 18+ and npm
- Python 3.9+
- MySQL 8 running on port `3306`
- (Optional) Gmail app password for OTP emails, Razorpay test keys, Firebase project for Google sign-in

### 1. Clone

```bash
git clone https://github.com/Annepuuday111/GigShield-AI-Gig-Insurance.git
cd GigShield-AI-Gig-Insurance
```

### 2. Create the database

```sql
CREATE DATABASE ai_insurance;
```

### 3. Configure environment

The backend reads these environment variables (see `backend/src/main/resources/application.properties`); export them in your shell before starting:

```bash
export SPRING_DATASOURCE_URL=jdbc:mysql://localhost:3306/ai_insurance
export SPRING_DATASOURCE_USERNAME=root
export SPRING_DATASOURCE_PASSWORD=your_mysql_password
export MAIL_USERNAME=your_email@gmail.com
export MAIL_PASSWORD=your_gmail_app_password
export RAZORPAY_KEY_ID=your_razorpay_test_key_id
export RAZORPAY_KEY_SECRET=your_razorpay_test_secret
export AI_SERVICE_URL=http://localhost:8000
export FRONTEND_URL=http://localhost:5173
```

Create `frontend/.env`:

```env
VITE_API_URL=http://localhost:4000
VITE_FIREBASE_API_KEY=your_firebase_api_key
VITE_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=your_project_id
VITE_FIREBASE_STORAGE_BUCKET=your_project.appspot.com
VITE_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
VITE_FIREBASE_APP_ID=your_app_id
```

### 4a. One-command start

```bash
chmod +x start.sh
./start.sh        # macOS / Linux
start.bat         # Windows
```

The script frees ports `8000`, `4000` and `5173`, creates a Python venv for the AI service, builds and runs the Spring Boot API, installs and starts the frontend. Press `Ctrl+C` to stop everything.

### 4b. Or start each service manually

```bash
# AI service  → http://localhost:8000  (Swagger UI at /docs)
cd ai-model
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
uvicorn main:app --host 0.0.0.0 --port 8000

# Backend     → http://localhost:4000
cd backend
mvn spring-boot:run

# Frontend    → http://localhost:5173
cd frontend
npm install
npm run dev
```

On first start the backend creates a default admin account (see `AdminInitializer.java`) – change its credentials from the admin panel.

### 🐳 Docker

Both `backend/` and `ai-model/` include a `Dockerfile`:

```bash
docker build -t gigshield-backend ./backend
docker build -t gigshield-ai ./ai-model
```

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 📸 Screenshots

<div align="center">

**🌍 Landing Page**

<img src="assets/landing_page.png" alt="Landing page" width="850"/>

**🛵 Worker Dashboard**

<img src="assets/user_dashboard.png" alt="Worker dashboard" width="850"/>

**👑 Admin Dashboard**

<img src="assets/admin_dashboard.png" alt="Admin dashboard" width="850"/>

**📝 Register**

<img src="assets/register.png" alt="Register page" width="850"/>

**🔐 Login**

<img src="assets/login.png" alt="Login page" width="850"/>

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 🗺️ Roadmap

- [x] Weekly plans with AI-adjusted premiums
- [x] Scheduled parametric auto-claims & fraud scoring
- [x] Razorpay payments and wallet payouts
- [ ] Replace mock weather with a live weather / AQI API
- [ ] ML-based fraud model trained on claim history
- [ ] Mobile app for delivery partners

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push the branch: `git push origin feature/your-feature`
5. Open a Pull Request

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 👨‍💻 Author

<div align="center">

### Annepu Uday Kumar

<a href="https://github.com/Annepuuday111"><img src="https://img.shields.io/badge/GitHub-Annepuuday111-845EF7?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
<a href="https://annepuudaykumar.netlify.app"><img src="https://img.shields.io/badge/Portfolio-Visit-FF6B6B?style=for-the-badge&logo=netlify&logoColor=white" alt="Portfolio"/></a>

</div>

<br/>

<div align="center">⭐ If you like this project, give it a star!</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:845EF7,35:4DABF7,70:FFA94D,100:FF6B6B&height=120&section=footer" width="100%"/>
