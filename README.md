<!-- Header Section -->
<div align="center">
  
![Profile Banner](https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=30&duration=2200&pause=1200&color=00B8D4&center=true&vCenter=true&width=700&lines=Shreya+Jagtap;Backend+%26+System+Design+Focused;Building+Production-Grade+Systems;Scalable+Architecture+%7C+Distributed+Thinking)

**Focused on backend engineering, scalable architecture, distributed systems, and production-grade system design through hands-on large-scale application development.**

</div>

---

## 🚧 Current Focus Areas

<div align="center">

| Area | Focus |
|------|-------|
| **Backend Engineering** | Production-grade API architecture |
| **System Design** | Feed systems, scalability, consistency tradeoffs |
| **Distributed Systems** | Storage lifecycle, async workflows, caching patterns |
| **Databases** | Query optimization, pagination, transactional integrity |
| **Infrastructure** | Redis, PostgreSQL, MinIO, containerized environments |
| **Current Project** | Instagram-scale backend system built from scratch |

</div>

---

## 👨‍💻 About Me

I’m focused on backend engineering and production-grade system design, building large-scale backend systems to deeply understand scalability, distributed-system fundamentals, transactional consistency, and real-world architecture tradeoffs through hands-on implementation.

My current work centers around designing an Instagram-scale backend architecture covering authentication systems, social graph modeling, media storage pipelines, feed systems, caching strategies, lifecycle management, scalable API design, and infrastructure-oriented backend development.

I’m actively exploring distributed systems, scalable backend architecture, infrastructure engineering, and eventually microservices-based system design as part of building larger-scale backend ecosystems. I also maintain an interest in AI/ML as a future complementary domain alongside backend systems engineering.

**Location:** India

## 🎓 Education & Learning Focus

| Category | Details |
|----------|---------|
| **Education** | Computer Science & backend systems focused learning |
| **Primary Focus** | Backend engineering, scalable systems, distributed-system fundamentals |
| **Currently Exploring** | Feed systems, infrastructure design, caching strategies, storage architecture |
| **Future Direction** | Distributed systems, microservices architecture, AI/ML integration awareness |

## 💻 Core Technical Stack

### **Languages**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)


### **Backend & Infrastructure**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![MinIO](https://img.shields.io/badge/MinIO-C72E49?style=for-the-badge&logo=minio&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![S3 Compatible](https://img.shields.io/badge/S3-Compatible_Storage-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white)

### Engineering Interests
- Distributed Systems
- Event-Driven Architecture
- Scalable Backend Infrastructure
- Microservices Architecture
- Storage Systems & Caching
- System Design & Reliability
- Applied AI/ML Systems (Future Exploration)

---

## 🚀 Currently Building

### **Instagram-Scale Backend System**
> A production-grade backend architecture focused on scalability, distributed-system fundamentals, storage workflows, and high-scale social platform design.

<div align="left">

**Core Architecture Areas:**
- Authentication, session lifecycle, and security systems
- Social graph modeling with privacy-aware visibility enforcement
- Media upload pipelines with signed URL storage architecture
- Feed system design with scalable pagination and filtering strategies
- Transaction-safe engagement systems (likes, comments, notifications)
- Storage lifecycle management, cleanup orchestration, and async processing foundations

**Engineering Focus:**
- Scalable backend architecture & distributed-system fundamentals
- Query optimization, transactional consistency, and concurrency control
- Object storage workflows, caching strategies, and infrastructure-oriented backend design
- Production-grade API architecture and system reliability patterns

**Current Stack:** Python • FastAPI • PostgreSQL • Redis • MinIO • Docker

**GitHub Repo:** [`instagram-backend`](https://github.com/shreyajagtap758-sys/instagram-backend)

</div>

---

### **🧠 Ongoing Engineering Exploration**
> Continuously studying backend scalability patterns, distributed-system concepts, and production architecture tradeoffs through hands-on implementation and system-focused projects.

**Current Areas of Exploration:**
- Feed fanout strategies & scalable pagination
- Distributed-system design patterns
- Event-driven architecture foundations
- Storage systems, caching, and lifecycle orchestration
- Backend infrastructure and reliability engineering
- Applied AI/ML systems as a future complementary engineering domain

**Focus:** Building strong backend/system-design depth through implementation-first learning rather than isolated theory.

---

## 🏗️ Architecture Decisions & Engineering Tradeoffs

<details>
<summary><b>📦 Direct-to-Storage Media Architecture</b></summary>

**Problem:**  
How can large media uploads scale efficiently without routing files through the backend server?

**Approach:**
- Generate signed upload URLs for direct client uploads
- Keep storage buckets private
- Validate object ownership and existence before post creation
- Use signed access URLs for controlled media rendering

**Why This Design:**
- Backend never handles raw media bytes
- Reduces API server bandwidth and memory pressure
- Scales storage independently from application servers
- Maintains secure access control over uploaded media

</details>

<details>
<summary><b>🔐 Refresh Token Rotation & Reuse Detection</b></summary>

**Problem:**  
How can refresh tokens remain secure against replay attacks and token theft?

**Approach:**
- Single-use refresh token rotation
- Atomic token invalidation
- Reuse detection with cascading session invalidation
- Redis-backed blacklist for revoked access tokens

**Why This Design:**
- Prevents replay attacks
- Limits stolen-token lifespan
- Maintains strong session consistency across devices

</details>

<details>
<summary><b>📄 Snapshot-Consistent Cursor Pagination</b></summary>

**Problem:**  
How can pagination remain stable while new posts are being created concurrently?

**Approach:**
- Cursor-based pagination using `created_at DESC, id DESC`
- Snapshot timestamp freezing
- Deterministic ordering across requests

**Why This Design:**
- Prevents duplicate or skipped results during pagination
- Avoids expensive offset-based scans
- Supports scalable feed-style querying patterns

</details>

<details>
<summary><b>🗑️ Media Lifecycle & Cleanup Architecture</b></summary>

**Problem:**  
How should abandoned uploads and deleted media be handled safely?

**Approach:**
- Upload lifecycle tracking (`pending → attached`)
- Soft delete with delayed retention window
- Retry-safe orphan cleanup workflows
- Delayed hard-delete storage cleanup

**Why This Design:**
- Prevents orphaned storage objects
- Reduces accidental permanent deletion risk
- Separates request lifecycle from cleanup workflows

</details>

---

## 🧩 Problem Solving & DSA

**LeetCode:** [View Profile](https://leetcode.com/R9Sz5tXVxg)

**Problem-Solving Focus:**
- Pattern-oriented DSA learning and problem decomposition
- Strong focus on arrays, hashing, sliding window, binary search, graphs, and backend-relevant data structures
- Emphasis on scalability thinking, optimization tradeoffs, and clean implementation strategies
- Consistent practice to strengthen system-level problem-solving and engineering intuition

**Current Direction:**
Using DSA and algorithmic thinking to build stronger foundations for backend engineering, scalable systems, and production-grade architecture design.

---

## 📚 Open Source & Community Goals

**Current Direction:**
- Building production-grade backend systems to strengthen real-world engineering depth
- Preparing to contribute to backend and infrastructure-focused open-source ecosystems
- Exploring contribution opportunities in FastAPI, SQLAlchemy, Redis-related tooling, and backend architecture projects

**Contribution Interests:**
- Backend frameworks & API architecture
- Database and ORM tooling
- Scalable system design patterns
- Infrastructure-oriented backend workflows
- Developer tooling and performance optimization

**Upcoming Goal:**  
Actively working toward meaningful open-source contributions through backend-focused projects and production-oriented engineering work.

---

## 📝 Technical Writing & Engineering Notes

I’m interested in documenting backend architecture decisions, scalability tradeoffs, and production-oriented engineering concepts through practical system-building experiences and implementation-focused notes.

**Planned Topics:**
- Authentication & session security architecture
- Feed system design and pagination strategies
- Rate limiting algorithms and Redis workflows
- Storage lifecycle management and media pipelines
- Transaction consistency and concurrency control
- Backend scalability and infrastructure tradeoffs

**Future Goal:**  
Building a collection of backend engineering writeups and architecture breakdowns based on real implementation experiences from large-scale backend projects.

---

## 🎯 Interests & Focus Areas

### Engineering Interests
- Backend architecture & scalable system design
- Distributed systems and infrastructure engineering
- Storage systems, caching, and performance optimization
- Feed systems, consistency models, and reliability patterns
- Applied AI/ML systems as a future complementary domain

### Beyond Engineering
- Problem solving & algorithmic thinking
- Exploring large-scale technology architectures
- Reading about system design and backend engineering patterns
- Building long-term engineering depth through hands-on projects

---

## 📊 GitHub Activity

<div align="center">

![GitHub Stats](https://github-readme-stats.herokuapp.com/api?username=shreyajagtap758-sys&show_icons=true&theme=github_dark&hide_border=true&count_private=true)

</div>

---

## 📌 Featured Project

<div align="center">
Primary production-oriented backend systems project focused on scalability, distributed-system fundamentals, and backend architecture design.

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=shreyajagtap758-sys&repo=instagram-backend&theme=github_dark&hide_border=true)](https://github.com/shreyajagtap758-sys/instagram-backend)

</div>

---

## 🔗 Connect & Collaborate

I’m always interested in connecting with people working on:
- Backend engineering & scalable system design
- Distributed systems and infrastructure architecture
- Production-grade backend projects
- Open-source backend ecosystems
- Engineering discussions around scalability, reliability, and system tradeoffs

### Profiles
- GitHub: https://github.com/shreyajagtap758-sys
- LeetCode: https://leetcode.com/u/R9Sz5tXVxg/
- LinkedIn: https://linkedin.com/in/ShreyaJagtap

---

<div align="center">

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:shreyajg.connect@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/shreyajagtap758-sys)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/u/R9Sz5tXVxg/)

</div>

---

**Last Updated:** Automatically maintained through GitHub workflows
