<div align="center">

# Hi, I'm Gyanendra Pratap Singh 👋

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=500&size=22&pause=1000&color=0E75B6&center=true&vCenter=true&width=650&lines=Backend+Developer+%7C+Python+%2F+Django+%2F+FastAPI;Multi-Tenant+SaaS+%26+Distributed+Systems;Agentic+AI+%E2%80%94+LLM+Tool-Calling+%2F+RAG" alt="Typing SVG" />

<img src="https://komarev.com/ghpvc/?username=gyanendra-hash&label=Profile%20views&color=0e75b6&style=flat" alt="Profile views" />

</div>

<br/>

## 🧭 About Me

I build backend systems and APIs — from multi-tenant SaaS platforms to distributed
microservices — mostly in Python with Django and FastAPI.

- 🔭 Currently working at **Ednectar**
- 🌱 Currently deepening my skills in:
  - Distributed systems fundamentals — rate limiting, task scheduling, leader election
  - Agentic AI / LLM tool-calling and RAG pipelines
  - Docker, Redis, and Celery for async/background workloads
- 📚 Maintaining a private interview-prep knowledge base — DSA, System Design
  (LLD/HLD: 24 design patterns + 26 real-world systems), and deep-dive
  Python/Django/DRF/FastAPI tracks, each with theory, diagrams, and working code
- 👯 Open to collaborating on **backend & SaaS projects (Django / FastAPI)**
- 🤝 Looking for input on scaling multi-tenant SaaS applications and optimizing
  Django/FastAPI microservices
- 💬 Ask me about Python, Django, FastAPI, REST/GraphQL APIs, payment gateway
  integrations (CC Avenue, Stripe, Razorpay), and Redis-backed real-time systems
- 📫 Reach me at **gyanendragps666@gmail.com**

<br/>

## 🛠️ Tech Stack

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white" alt="Django" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" />
  <img src="https://img.shields.io/badge/Django%20REST-ff1709?style=for-the-badge&logo=django&logoColor=white" alt="Django REST Framework" />
  <img src="https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white" alt="Celery" />
</p>
<p>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" />
</p>
<p>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white" alt="Nginx" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" />
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white" alt="JWT" />
  <img src="https://img.shields.io/badge/Razorpay-02042B?style=for-the-badge&logo=razorpay&logoColor=white" alt="Razorpay" />
</p>
<p>
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" alt="LangGraph" />
  <img src="https://img.shields.io/badge/pgvector-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="pgvector" />
  <img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white" alt="OpenAI" />
</p>

<br/>

## 💼 Featured Projects

### 🤖 [AgentOps](https://github.com/gyanendra-hash/AgentOps)
Distributed API gateway, task scheduler, and agentic AI ops layer — a microservice
platform combining a Redis-backed rate limiter, an API gateway, a priority- and
dependency-aware task scheduler, a worker pool, and a LangGraph-based control
plane that schedules jobs, answers operational questions, and debugs failures
using RAG over system logs and runbooks.

- Six independently deployable FastAPI services, each owning its own data store
- Token Bucket & Sliding Window rate limiting as atomic Redis Lua scripts,
  verified under concurrent load with Locust; DAG-based job scheduling
  (Kahn's algorithm) with Redis-backed leader election
- A pgvector-backed RAG layer for incident debugging, LLM tool-calling with a
  human-in-the-loop confirmation gate for destructive actions, and intent-routed
  multi-agent orchestration (schedule / debug / monitor)
- Always-on per-node latency/token tracing with optional Langfuse export, plus
  an eval harness for intent-routing accuracy
- **All six planned milestones shipped end to end; 174 tests, all run against
  fakes/mocks** — no Docker, downloaded model, or LLM key required to run the suite

<p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/Docker%20Compose-2496ED?style=flat-square&logo=docker&logoColor=white" alt="" />
</p>

### 🎓 [Institute SaaS Backend](https://github.com/gyanendra-hash/institute-saas-backend)
Multi-tenant Django + DRF backend for coaching institutes — one codebase, many
institutes, each fully data-isolated at the ORM level.

- Tenant-scoped default model manager enforces isolation automatically — no
  query can accidentally leak data across tenants
- JWT auth with tenant + role embedded in the token; students & batches, bulk
  attendance marking + reports, fee management (Razorpay checkout + async PDF
  receipts + outstanding-dues reporting), and an exam/result module with
  auto-calculated rank/average/pass-fail
- Async notifications via Celery + Redis; free-tier deployable on Render + Neon

<p>
  <img src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/DRF-ff1709?style=flat-square&logo=django&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/Razorpay-02042B?style=flat-square&logo=razorpay&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="" />
</p>

### 📊 [Education Analytics Platform](https://github.com/gyanendra-hash/education-analytics)
A full-stack analytics application for educational institutions: ETL pipelines
that consolidate multi-source student data into PostgreSQL, a FastAPI backend, and
interactive Plotly dashboards for real-time, data-driven decisions.

- Microservice-oriented FastAPI backend with dual storage — PostgreSQL for
  structured data, MongoDB for semi-structured data
- Automated ETL pipelines and predictive analytics for student outcomes
- JWT authentication, role-based access control, full Docker Compose setup

<p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white" alt="" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="" />
</p>

### 💳 Multi-Tenant SaaS Platform (Django) — *private repository*
A Django monolith combining multi-tenancy, an LMS module, and a crowdfunding module
in one codebase, backed by Redis-driven async task processing.

- Tenant isolation, LMS, and crowdfunding domains sharing a common Django core
- Async task handling via Celery + Redis, containerized with Docker

Also built **AES-encrypted CC Avenue payment flows** (checkout, success, and
cancel handling with secure transaction verification end to end) into a
Django/FastAPI backend.

<br/>

## 📡 Connect with Me

<p>
<a href="https://in.linkedin.com/in/gyanendra-pratap-singh-310563377" target="_blank">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>
<a href="mailto:gyanendragps666@gmail.com">
  <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
</a>
</p>

<br/>

## 📈 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=gyanendra-hash&show_icons=true&locale=en&theme=default" alt="GitHub Stats" height="165" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=gyanendra-hash&show_icons=true&locale=en&layout=compact" alt="Top Languages" height="165" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=gyanendra-hash" alt="GitHub Streak" />
</p>
