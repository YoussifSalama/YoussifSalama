<div align="center">

# Hi, I'm Youssif Salama 👋

### Full-Stack Engineer · Marketplaces, Fintech & AI Integration

I build the backend logic that sits between two-sided systems that don't trust each other by default —
matching engines, wallets, and state machines where money and timing have to reconcile correctly.

[![Email](https://img.shields.io/badge/Email-youssifsalama01%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:youssifsalama01@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-youssif--salama-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/youssif-salama-039506244/)
[![Location](https://img.shields.io/badge/Cairo%2C_Egypt-Remote_Worldwide-2E8B57?style=for-the-badge&logo=googlemaps&logoColor=white)](#)

</div>

<br>

## 🧩 About Me

Full-stack developer shipping production systems across **fintech, marketplaces, and AI-powered products**. I've built a logistics marketplace backend (supply/demand matching, offer handling, trip lifecycle, and the financial edge cases that come with real money and real timing), a fintech e-wallet with real-time transaction processing, an AI-powered social platform on the MERN stack (**98/100** at graduation), and a string of bilingual, CMS-driven Next.js platforms. I also integrate **OpenAI GPT-4, ElevenLabs Voice AI, and Google Gemini** into production systems with real latency and cost constraints, and spent a year teaching backend engineering to 30+ developers per cohort.

📍 Cairo, Egypt &nbsp;·&nbsp; 🌍 Open to Full-Time Remote (Worldwide) &nbsp;·&nbsp; ⚡ Immediate Start &nbsp;·&nbsp; ✅ Military Service Exempt

<br>

## 🛠️ Tech Stack

<div align="center">

**Backend**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white)
![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=flat-square&logo=socket.io&logoColor=white)

**Frontend**

![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vue.js&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

**Data & Infra**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)

**AI Integration**

![OpenAI](https://img.shields.io/badge/OpenAI_GPT--4-412991?style=flat-square&logo=openai&logoColor=white)
![Gemini](https://img.shields.io/badge/Google_Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![ElevenLabs](https://img.shields.io/badge/ElevenLabs_Voice_AI-000000?style=flat-square)

</div>

<br>

## 🚀 Projects

<br>

### 🚚 Wasel — Logistics & Fleet Marketplace
**Role:** Backend Developer &nbsp;|&nbsp; 🔗 [wasel-fleet.com](https://wasel-fleet.com/) &nbsp;|&nbsp; ⭐ Flagship project

![NestJS](https://img.shields.io/badge/-NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/-Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Redis](https://img.shields.io/badge/-Redis%2FBullMQ-DC382D?style=flat-square&logo=redis&logoColor=white)
![Socket.io](https://img.shields.io/badge/-Socket.IO-010101?style=flat-square&logo=socket.io&logoColor=white)
![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![AWS S3](https://img.shields.io/badge/-AWS%20S3-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Twilio](https://img.shields.io/badge/-Twilio-F22F46?style=flat-square&logo=twilio&logoColor=white)

A logistics marketplace connecting customers who need truck transport with drivers who bid offers, plus a full admin back office.

- Customer requests a shipment → drivers submit offers → trip lifecycle tracked in real time.
- Built the state machine tying trip status to financial logic: timing-dependent refunds, mid-trip cancellations, and wallet-balance-to-transaction-log reconciliation.
- Admin back office manages users, drivers, trips, storage owners, finance/payouts, identity verification, blog content, analytics, and platform settings.
- **Backend (`wasel-backend`):** NestJS + Prisma + PostgreSQL, Redis-backed job queues (BullMQ), Socket.IO gateways for live trip/notification updates, S3 file storage, 2FA/OTP (otplib), SMS via Twilio, email via Nodemailer/Handlebars, Excel export, Swagger docs.
- **Dashboard (`wasel-dashboard`):** React + Vite, Tiptap + Monaco editors, real-time updates via Socket.IO client, Recharts.
- **Frontend (`wasel-fe`):** Next.js, i18n, GSAP + Lenis smooth scroll, Lottie, Zustand.
- 🏆 **Highlight:** the only project in the portfolio running a full NestJS + PostgreSQL + Redis stack with real-time features and 2FA — production-grade backend engineering vs. the simpler Express/MongoDB APIs elsewhere.

<br>

### 🤖 Plato — AI Recruiting & Hiring Platform
**Role:** AI Integration Engineer &nbsp;|&nbsp; 🔗 [agency.platohiring.com](https://agency.platohiring.com/)

![NestJS](https://img.shields.io/badge/-NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Prisma](https://img.shields.io/badge/-Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Redis](https://img.shields.io/badge/-Redis%2FBullMQ-DC382D?style=flat-square&logo=redis&logoColor=white)
![OpenAI](https://img.shields.io/badge/-OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Stripe](https://img.shields.io/badge/-Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white)
![ElevenLabs](https://img.shields.io/badge/-ElevenLabs%20TTS-000000?style=flat-square)

An AI-powered hiring platform with two sides — agencies sourcing and screening candidates, and candidates applying and interviewing — plus an admin layer and a Chrome extension for resume capture.

- Two distinct resume pipelines: an **agency upload pipeline** (PDF/DOCX → BullMQ job → parse → OpenAI batch analysis → structured AI output written to the DB) and a **connector ingestion pipeline** (REST/S3/signed-URL/DB sources → multi-stage discover → download → parse → AI-snapshot → score pipeline).
- Built OpenAI key rotation so the platform round-robins across multiple API keys under load instead of hammering a single key.
- Implemented a subscription/quota system (intro/base/pro/enterprise plans) enforced transactionally to prevent race conditions on concurrent usage.
- Integrated ElevenLabs TTS for AI-driven candidate calls, plus Stripe billing and a Chrome extension that authenticates against the agency dashboard and talks to the backend API.
- **Backend:** NestJS + Prisma, Redis-backed BullMQ queues across five dedicated workers, JWT guards separating agency/candidate/admin/anonymous-session access, Swagger docs split by audience (`/api/agency`, `/api/candidate`).
- 🏆 **Highlight:** the pipeline architecture explicitly separates synchronous AI scoring (fast, per-candidate) from batched AI analysis (cost-efficient, bulk) — a deliberate latency-vs-cost tradeoff baked into the system design.

<br>

### 🏗️ AMF — Corporate Website with Custom CMS
**Role:** Full Stack Developer (team) &nbsp;|&nbsp; 🔗 [amf.com.eg](http://amf.com.eg/en)

![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![Firebase](https://img.shields.io/badge/-Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![Redux](https://img.shields.io/badge/-Redux%20Toolkit-764ABC?style=flat-square&logo=redux&logoColor=white)
![Express](https://img.shields.io/badge/-Express.js-000000?style=flat-square&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)

Corporate/industrial site for an Arabtec-linked client.

- Company marketing site with content managed through a custom admin CMS.
- **Frontend (`AMF`):** Next.js, next-intl (i18n), Firebase, GSAP animations, Swiper carousels, Zustand, transactional email via Nodemailer.
- **CMS (`AMF-CMS`):** React + Vite, Redux Toolkit, full Tiptap suite with collaboration cursors, drag-drop uploads.
- **Backend (`AMF-CMS-BACKEND`):** Express + MongoDB (Mongoose), Helmet-hardened API.
- Implemented Next.js SSR and SSG for fast page delivery and strong SEO, with dynamic routing driven entirely by CMS content.

<br>

### 🚪 Opindoo — Product Website & Dashboard
**Role:** Full Stack Developer (team) &nbsp;|&nbsp; 🔗 [opindoo.com](https://opindoo.com/en)

![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![Prisma](https://img.shields.io/badge/-Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![MUI](https://img.shields.io/badge/-MUI%20%2B%20Radix-007FFF?style=flat-square&logo=mui&logoColor=white)
![NextAuth](https://img.shields.io/badge/-NextAuth.js-000000?style=flat-square)

"Where windows & doors meets top quality" — a product showcase site for a windows & doors manufacturer/retailer.

- Product catalog with gallery and showroom pages, 360°/panoramic product views, quote/contact requests, and admin content management — all in a single Next.js app.
- Tech: Next.js + Prisma + MongoDB + NextAuth (credentialed admin login), MUI + Radix UI, react-360-view and react-photo-sphere-viewer for immersive product views, Tiptap rich text, i18next, Firebase, Nodemailer.
- 🏆 **Highlight:** merges storefront and admin into a single codebase using Next.js route groups (`/admin`).
- Redesigned the corporate site and overhauled the admin dashboard, extending the codebase across frontend UI and backend APIs to improve platform reliability.

<br>

### 🎨 Sci-Fi — Edutainment Booking & CMS Platform
**Role:** Full Stack Developer (team)

![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![Express](https://img.shields.io/badge/-Express.js-000000?style=flat-square&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Zod](https://img.shields.io/badge/-Zod-3E67B1?style=flat-square&logo=zod&logoColor=white)
![Firebase](https://img.shields.io/badge/-Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)

Edutainment company site — nursery enrollment, school-trip bookings, land/plot listings, an online store, and company profile info.

- Public marketing/booking site plus a full admin CMS and API to manage all of it.
- **Frontend (`sci-fi-fe`):** Next.js, i18n, GSAP + fullPage.js scroll sections, Swiper/Embla carousels, lightbox galleries, scheduled jobs (node-cron), Tiptap content rendering.
- **CMS (`sci-fi-cms`):** React + Vite, Monaco code editor, JWT auth, Zod-validated forms, image cropping, Firebase storage.
- **Backend (`sci-fi-be`):** Express + MongoDB (Mongoose), JWT auth, bcrypt password hashing, Zod schema validation.

<br>

### 🛍️ Hatly Store — E-Commerce Platform
**Role:** Full Stack Developer (team) &nbsp;|&nbsp; 🔗 [hatlystore.com](https://www.hatlystore.com/) *(current live site — new version in development)*

![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![JWT](https://img.shields.io/badge/-JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)
![Zustand](https://img.shields.io/badge/-Zustand-433E38?style=flat-square)
![Firebase](https://img.shields.io/badge/-Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)

A Next.js e-commerce storefront: product browsing, cart, checkout flow, user accounts, order history, and sharing.

- Explicitly built with SOLID principles and OOP patterns for maintainability (single-responsibility components/services).
- Full bilingual EN/AR support, RTL-aware via next-intl.
- Tech: Next.js, JWT auth (jsonwebtoken/jwt-decode), Firebase, GSAP, Embla/Swiper carousels, react-hook-form + Zod validation, Tiptap, Zustand, next-themes (dark mode), and a web-scraping utility (cheerio).

<br>

### 💳 Lite Pay — E-Wallet Platform
**Role:** Backend Developer (team) &nbsp;|&nbsp; 🔗 [litepay-eg.net](https://www.litepay-eg.net)

![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/-Express.js-000000?style=flat-square&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![WebSockets](https://img.shields.io/badge/-WebSockets-010101?style=flat-square&logo=socket.io&logoColor=white)

A secure e-wallet platform with real-time transaction processing.

- Server-side architecture for account management, wallet balance tracking, and transaction-history APIs.
- Real-time WebSocket endpoints for live transaction status — instant feedback on deposits, withdrawals, and P2P transfers.
- Integrated third-party payment gateway APIs with webhook verification and idempotency to prevent duplicate transactions.
- OAuth 2.0 and JWT authentication with RBAC and API rate limiting to protect financial endpoints.

<br>

### 🤝 Tech Bridge — AI Social & Jobs Platform
**Role:** Full Stack Developer & Team Lead &nbsp;·&nbsp; 🎓 Graduation Project — **98/100**

![MERN](https://img.shields.io/badge/-MERN%20Stack-47A248?style=flat-square&logo=mongodb&logoColor=white)
![AI](https://img.shields.io/badge/-NLP%20%2F%20AI%20Models-412991?style=flat-square&logo=openai&logoColor=white)

An AI-powered social media and job-matching platform with an assistant for content quality and automated moderation.

- Led full-stack development of the platform end to end.
- Integrated NLP-based AI models for post optimisation and inappropriate-content detection, achieving **94% moderation accuracy** on test datasets.
- Designed a scalable architecture allowing the AI moderation pipeline to deploy and scale independently from the core social platform.

<br>

## 💼 Experience

| Role | Company | Period |
|---|---|---|
| AI Integration Engineer (Part-time) | Plato | Dec 2025 – Present |
| Full Stack Developer | Trendlix | Aug 2025 – Present |
| Backend Instructor | MBD Academy | Aug 2024 – Aug 2025 |
| Front End Vice Head (Mentor) | GDSC · Damanhour University | Oct 2023 – Jul 2024 |
| Backend Developer (Internship) | Route IT Training Centre | Nov 2023 – Mar 2024 |
| Front End Developer (Internship) | Minplan International | Apr 2023 – Jul 2023 |

<br>

## 🎓 Education

**B.Sc. Computer Science & Information Technology** — Damanhour University, Egypt &nbsp;·&nbsp; GPA 3.2/4.0
Graduation Project: Tech Bridge — AI-powered social and jobs platform, highest faculty score (98/100).

<br>

<div align="center">

### 📫 Let's talk

[![Email](https://img.shields.io/badge/Email_me-youssifsalama01%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:youssifsalama01@gmail.com)
[![LinkedIn](https://img.shields.io/badge/Connect_on-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/youssif-salama-039506244/)

</div>
