<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=240&text=Suraj%20Khonde&fontAlign=50&fontAlignY=35&desc=Backend%20Engineer%20(Node.js)%20%7C%20Scalable%20APIs%20%7C%20Redis%20%7C%20SQL&descAlign=50&descAlignY=55&color=0:0ea5e9,100:22c55e" alt="header" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/surajrkhonde/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-surajrkhonde-0A66C2?logo=linkedin&logoColor=white" /></a>
  <a href="mailto:surajrkhonde@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-surajrkhonde%40gmail.com-EA4335?logo=gmail&logoColor=white" /></a>
  <a href="https://surajkhonde.github.io/"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-Live-111827?logo=vercel&logoColor=white" /></a>
  <a href="https://medium.com/@surajrkhonde"><img alt="Medium" src="https://img.shields.io/badge/Blogs-Medium-000000?logo=medium&logoColor=white" /></a>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&pause=900&center=true&vCenter=true&width=720&lines=Backend+Engineer+%7C+Node.js+%7C+Distributed+Systems;Scalable+APIs+%7C+Caching+%7C+Async+Processing;Production+Debugging+%26+Performance+Mindset;Currently%3A+System+Design+Deep+Dive" alt="typing" />
</p>

---

## 👋 About Me

Backend Engineer with 3+ years of experience building and operating production systems using Node.js.

### What I focus on
- Designing scalable REST APIs  
- Structuring asynchronous workflows  
- Implementing reliable background processing  
- Database optimization (MongoDB / MySQL)  
- Caching strategies using Redis  

### How I work
I take end-to-end ownership of backend components — from architecture and implementation to production debugging and performance tuning.

I prioritize clean design, predictable system behavior, and long-term maintainability.

While I can contribute across the stack when needed, my strength lies in backend architecture, scalability, and building stable, production-ready services.
---
## 🧰 Core Tech Stack

**Backend**
- Node.js · Express
- MongoDB · MySQL
- Redis (caching & async coordination)
- REST APIs · Background Jobs · WebSockets

**Infrastructure & Dev**
- Docker · AWS (EC2)
- Git · Linux
- Postman

**Frontend (when required)**
- React · Next.js
- TailwindCSS
---

## 🚀 Selected Projects

### 🔹 Chatty – Backend Monolith
**Node.js · Express · MongoDB · Socket.IO**

Backend-first chat system demonstrating clean API design, authentication flow, and real-time communication patterns. Structured for scalability and production-style organization.

[Repository](https://github.com/SurajKhonde/Chatty_backend_monolith)

---

### 🔹 Freelanzio – Microservices (WIP)
**Node.js · Docker · Service Boundaries**

Work-in-progress microservice architecture exploring service separation, async communication patterns, and scalable system design concepts.

[Repository](https://github.com/SurajKhonde/Freelanzio)

---

### 🔹 jobber-shared (NPM Package)
**Node.js · TypeScript · Shared Contracts**

Reusable shared utilities package for validation, error handling, and service contracts — designed to improve consistency across services.

[Repository](https://github.com/SurajKhonde/jobber-shared)

---

### 🔹 MovieReview
**React · Node.js · MongoDB**

Full-stack application with media upload, authentication, and structured API integration. Demonstrates clean client-server interaction and backend data handling.

[Repository](https://github.com/SurajKhonde/MovieReview)

---

### 🔹 Engineering Handbook

Structured backend, system design, SQL, and DSA notes focused on building strong engineering fundamentals.

[Repository](https://github.com/SurajKhonde/Engineering_Handbook)

---

## 🧠 Currently Strengthening

- Scalable system design (caching, async flows, load patterns)
- SQL optimization (indexing, execution plans, pagination)
- Distributed system fundamentals
- Data structures & algorithms

---

## 🗺️ One small architecture

<details>
  <summary><b>Click to view</b></summary>

```mermaid
flowchart LR
FE["Frontend (React)"] -->|"HTTP REST"| API["Express API (port 5000)"]
FE -->|"Socket.IO"| API

API -->|"Read/Write"| Mongo[(MongoDB)]
API -->|"Cache reads/writes"| Redis[(Redis)]

API -->|"Enqueue jobs"| Bull["Bull queues (Redis)"]
Bull -->|"Process jobs"| Workers["Background workers"]
Workers -->|"DB writes"| Mongo
Workers -->|"Emit realtime"| SIO["Socket.IO server"]
Workers -->|"Send email"| Email["Email (Ethereal dev / SendGrid prod)"]

API -->|"Uploads"| Cloudinary[(Cloudinary)]
Workers -->|"Uploads metadata"| Mongo
```

</details>

---

## 📈 GitHub cards

> These cards are powered by free third-party services, so they can sometimes rate-limit.
> If they don’t load, refresh once.

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=SurajKhonde&show_icons=true&hide_border=true&cache_seconds=86400" alt="github stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=SurajKhonde&layout=compact&hide_border=true&cache_seconds=86400" alt="top langs" />
</p>
<p align="center">
  <img height="180" src="https://streak-stats.demolab.com?user=SurajKhonde&hide_border=true" alt="streak" />
</p>

---

## 🤝 Open to

- Backend Engineering (Node.js) opportunities  
- Scalable API & distributed system development  
- Performance-critical and debugging-intensive environments

---

## 📬 Contact

- Email: **surajrkhonde@gmail.com**
- LinkedIn: https://www.linkedin.com/in/surajrkhonde/
- Portfolio: https://surajkhonde.github.io
- Medium: https://medium.com/@surajrkhonde

<p align="center">
  <i>Thanks for visiting — always happy to collaborate and build something useful.</i>
</p>
