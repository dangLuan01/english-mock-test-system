# 🎓 TOEIC/IELTS Online Testing & Learning Platform

🇻🇳 Vietnamese version: [README.vi.md](./README.vi.md)

---

A comprehensive **EdTech platform** designed to simulate standardized international exams such as **TOEIC** and **IELTS**.

The system focuses on:

- Minimal and modern Asian-inspired UI
- High performance & scalability
- Seamless user experience
- 24/7 reliability

The architecture follows a **Micro-repositories** approach to separate business domains for better maintainability and future scalability.

---

# 🏗 System Architecture (Repositories)

This repository serves as the central overview of the ecosystem.

The platform is separated into 3 independent repositories:

| Module | Description | Repository |
|---|---|---|
| API Server | RESTful backend API, scoring engine, exam session management, synchronization | `[API_Repo_Link](https://github.com/dangLuan01/ets-api)` |
| Client App | Student-facing frontend application for testing, practicing, and analytics | `[Client_Repo_Link](https://github.com/dangLuan01/ets-client)` |
| Admin Portal | CMS dashboard for managing exams, questions, and users | `[Admin_Repo_Link](https://github.com/dangLuan01/ets-admin)` |

---

# 🚀 Core Features

## Flexible Exam Engine

Supports multiple learning modes within a unified and adaptive interface.

### Exam Mode

Realistic exam simulation environment:

- 100–200 question full tests
- Standardized scoring flow
- Distraction-free experience

### Practice Mode

Micro-learning focused experience:

- Instant answer feedback
- Explanations and solutions
- Part-based practice

### Review Mode

Detailed exam review system:

- Review answer history
- Analyze strengths & weaknesses
- Track learning progress

---

## Seamless Cross-Device Experience

Real-time synchronization across devices:

- Start on mobile
- Continue on desktop
- No interrupted sessions

---

## Resilient Auto-Save

Intelligent auto-save mechanism:

- Zero-Data Loss architecture
- Handles:
  - Network failures
  - Browser crashes
  - Unexpected shutdowns

---

## Smart Revision

Integrated bookmark & revision system:

- Save important questions
- Personalized review workflow
- Foundation for spaced repetition algorithms

---

# 🛠 Architecture Highlights

## Data-Driven UI

Frontend architecture driven entirely by structured data.

Components dynamically adapt to:

- Full Exams
- Mini Tests
- Practice Parts

Benefits:

- Highly reusable components
- Minimal hard-coded layouts
- Easier feature expansion

---

## Optimized Database Writes

Backend optimized for massive concurrent answer submissions.

Techniques:

- Batching & Queueing
- Bulk Upsert operations
- Reduced database pressure
- Higher throughput performance

---

## Stateless & Scalable Backend

Backend services are designed to be stateless:

- Easy horizontal scaling
- Multi-instance deployment ready
- High traffic resilience

---

# 💻 Tech Stack

## Backend

- Go (Golang)
- Gin Framework

## Frontend

- React
- Next.js
- Zustand

## Database & Caching

- MySQL / PostgreSQL
- Redis

## DevOps & Deployment

- Docker
- Nginx
- GitHub Actions (CI/CD)
- Linux VPS
