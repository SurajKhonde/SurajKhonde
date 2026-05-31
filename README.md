<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=240&text=Suraj%20Khonde&fontAlign=50&fontAlignY=35&desc=Full%20Stack%20Engineer%20%7C%20Node.js%20%7C%20TypeScript%20%7C%20Production%20LLM%20Integration&descAlign=50&descAlignY=55&color=0:0ea5e9,100:22c55e" alt="header" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/surajrkhonde/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-surajrkhonde-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:surajrkhonde@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-Reach%20me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://pilooopu.shop"><img alt="Live product" src="https://img.shields.io/badge/Live-pilooopu.shop-22c55e?style=for-the-badge&logo=vercel&logoColor=white" /></a>
  <a href="https://medium.com/@surajrkhonde"><img alt="Medium" src="https://img.shields.io/badge/Writing-Medium-000000?style=for-the-badge&logo=medium&logoColor=white" /></a>
  <img alt="Profile views" src="https://komarev.com/ghpvc/?username=SurajKhonde&color=22c55e&style=for-the-badge&label=Profile+Views" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=900&center=true&vCenter=true&width=780&color=22C55E&lines=Full+Stack+Engineer+%7C+Node.js+%7C+TypeScript;Production+systems%3A+queues%2C+caching%2C+real-time;LLM+integration+behind+real+guardrails;Currently+shipping%3A+Pilooopu+%26+Dawa+Saathi" alt="typing" />
</p>

---

## About

Full Stack Engineer with **3+ years shipping production Node.js / TypeScript systems** — owning the full path from schema design to AWS deploy and CI/CD.

I'm equally at home on React / Next.js front ends, real-time WebSocket backends, queues, and caching, with hands-on **LLM integration via the Claude API (vision + text) behind production guardrails**. I care most about predictable system behaviour, clean design, and building things people in the real world actually use.

---

## 🚀 What I'm building right now

### 🔹 Pilooopu — Bulk Personalized WhatsApp Invite Platform
**`Node.js` · `TypeScript` · `BullMQ` · `Redis` · `PostgreSQL` · `Drizzle` · `Next.js` · `Puppeteer` · `WhatsApp Cloud API` · `Razorpay` · `Docker` · `Nginx`**

A live invite-card platform running at **[pilooopu.shop](https://pilooopu.shop)**.

- **Crash-resilient pipeline** — a 3-stage flow (render → upload → finalize) across 7 BullMQ queues, checkpointed in Redis. A worker crash resumes from the last completed step, not the start.
- **Privacy by default** — every guest phone encrypted with AES-256-CBC and a unique IV per record; decrypted only inside the send worker, masked as `+91*****1234` in every API response and log.
- **Smart retries** — retryable vs non-retryable errors are split, so bad data routes straight to a dead-letter queue instead of burning the 3-attempt budget.
- **Efficient rendering** — one reused Puppeteer browser produces both a 400×600 thumbnail and an 800×1200 full card from a single HTML pass.
- **Hardened API** — Redis-backed rate limiter with per-endpoint quotas and standard `X-RateLimit` headers; deployed as two Docker services (API + Worker) behind Nginx with graceful SIGTERM shutdown.

[Live](https://pilooopu.shop) · [Repository](https://github.com/SurajKhonde)

### 🔹 Dawa Saathi — AI Medicine-Awareness Telegram Bot
**`Node.js` · `TypeScript` · `Claude Vision + Text` · `Redis` · `PostgreSQL` · `openFDA` · `Telegram Bot API` · `Docker`**

A bot that reads a medicine-strip photo and returns an **elder-friendly drug summary** — built for people who find medicine labels hard to parse.

- Claude vision extracts the label at **~80% accuracy**, returned in plain, readable language.
- A **0.75 confidence gate** plus ingredient-only prompts refuse uncertain reads — cutting misleading or wrong drug info by **~80%**.
- Analyzed medicines are cached Redis → PostgreSQL, so repeat scans skip the model entirely — **~30% fewer tokens** and instant answers.
- Dockerized with health checks and graceful shutdown for one-command deploys.

[Try it](https://t.me/dawasaathi_bot) · [Repository](https://github.com/SurajKhonde)

---

## 💼 Experience

**Software Engineer — Advento Technologies, Hyderabad** · *Sep 2025 – Jan 2026*
Banking virtual-assistant platform. Built a WebSocket bot-to-agent escalation flow handling 1000+ concurrent sessions (handoff latency ↓ ~25%), moved uploads to presigned S3 URLs (server CPU ↓ ~40%), and set up CircleCI CI/CD with PM2 for near-zero-downtime releases.

**Full Stack Engineer — Technoloader Pvt Ltd, Jaipur** · *May 2024 – Jul 2025*
Real-time trading platform. Streamed filtered Binance market data over Socket.IO with Redis pub/sub fan-out, sustained 10K+ events/min under concurrent load, and offloaded reporting/notifications to BullMQ workers with retry/backoff to keep the price path fast.

**Full Stack Engineer — Avisirah Technologies, Hyderabad** · *Mar 2022 – Feb 2024*
Real-time social platform. Built feed and messaging APIs on Node/Express + MongoDB with Redis read-cache (p50 ↓ ~20%), JWT access/refresh auth with RBAC, and real-time chat, presence, and read receipts over Socket.IO.

---

## 🧰 Tech Stack

**Languages**
<p>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
</p>

**Backend**
<p>
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/Socket.IO-010101?style=for-the-badge&logo=socketdotio&logoColor=white" />
  <img src="https://img.shields.io/badge/BullMQ-EA2845?style=for-the-badge&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white" />
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white" />
</p>

**AI / LLM**
<p>
  <img src="https://img.shields.io/badge/Claude%20API-D97757?style=for-the-badge&logo=anthropic&logoColor=white" />
  <img src="https://img.shields.io/badge/Vision%20%2B%20Text-7C3AED?style=for-the-badge" />
  <img src="https://img.shields.io/badge/RAG-0EA5E9?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Confidence%20Gating-22C55E?style=for-the-badge" />
</p>

**Frontend**
<p>
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Redux%20Toolkit-764ABC?style=for-the-badge&logo=redux&logoColor=white" />
  <img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" />
</p>

**Databases**
<p>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Drizzle-C5F74F?style=for-the-badge&logo=drizzle&logoColor=black" />
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Firebase-DD2C00?style=for-the-badge&logo=firebase&logoColor=white" />
</p>

**Infra & DevOps**
<p>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white" />
  <img src="https://img.shields.io/badge/PM2-2B037A?style=for-the-badge&logo=pm2&logoColor=white" />
  <img src="https://img.shields.io/badge/CircleCI-343434?style=for-the-badge&logo=circleci&logoColor=white" />
  <img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black" />
</p>

---

## 🗺️ A system I run in production

<details>
  <summary><b>Pilooopu — crash-resilient invite pipeline</b></summary>

```mermaid
flowchart LR
  Client["Next.js client"] -->|REST| API["Express API (Docker)"]
  API -->|"Enqueue + checkpoint"| Redis[(Redis)]
  API -->|"Read / Write"| PG[(PostgreSQL · Drizzle)]

  Redis --> Q1["Queue 1: render"]
  Q1 --> Q2["Queue 2: upload"]
  Q2 --> Q3["Queue 3: finalize"]

  Q1 -->|"single reused browser"| PPTR["Puppeteer · thumb + full card"]
  Q2 -->|"asset upload"| Cloud[(Cloudinary)]
  Q3 -->|"AES-256 decrypt in worker"| WA["WhatsApp Cloud API"]

  API -. "bad data" .-> DLQ["Dead-letter queue"]
  Worker["Worker service (Docker)"] --> Redis
  Nginx["Nginx"] --> API
```

A worker crash resumes from the last completed checkpoint — render, upload, and finalize never repeat work that already succeeded.

</details>

---

## 📊 GitHub

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=SurajKhonde&show_icons=true&hide_border=true&title_color=22c55e&icon_color=0ea5e9&text_color=9f9f9f&bg_color=0d1117&cache_seconds=86400" alt="github stats" />
  <img height="170" src="https://streak-stats.demolab.com?user=SurajKhonde&hide_border=true&background=0D1117&stroke=0d1117&ring=22c55e&fire=0ea5e9&currStreakLabel=22c55e&sideLabels=9f9f9f&dates=6e7681" alt="streak" />
</p>

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=SurajKhonde&layout=compact&hide_border=true&title_color=22c55e&text_color=9f9f9f&bg_color=0d1117&langs_count=8&cache_seconds=86400" alt="top langs" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=SurajKhonde&bg_color=0d1117&color=22c55e&line=0ea5e9&point=ffffff&area=true&hide_border=true" alt="activity graph" />
</p>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=SurajKhonde&theme=algolia&no-frame=true&no-bg=true&margin-w=6&column=7" alt="trophies" />
</p>

> Cards are powered by free third-party services and can rate-limit occasionally — a refresh usually fixes it.

---

## 🤝 Open to

Full Stack / Backend roles (Node.js · TypeScript) where I can ship production systems and integrate AI in ways that hold up under real load and real users.

<p>
  <a href="mailto:surajrkhonde@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/surajrkhonde/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://surajkhonde.github.io"><img src="https://img.shields.io/badge/Portfolio-111827?style=for-the-badge&logo=githubpages&logoColor=white" /></a>
  <a href="https://medium.com/@surajrkhonde"><img src="https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white" /></a>
</p>

<img src="https://capsule-render.vercel.app/api?type=waving&section=footer&height=120&color=0:22c55e,100:0ea5e9" alt="footer" />
