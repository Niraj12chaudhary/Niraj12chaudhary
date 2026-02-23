# Shivam Kumar Chaudhary  
### Backend Systems Engineer | Distributed Systems | Production Architecture

I design and build backend systems that are resilient under load, safe with data, and predictable in failure.

My work focuses on multi-tenant SaaS platforms, asynchronous processing systems, and real-time distributed architectures. I care deeply about correctness, data integrity, and long-term maintainability over quick feature delivery.

---

## Engineering Focus

- Scalable backend services (NestJS, Fastify, Django)
- Multi-tenant SaaS architecture
- Asynchronous processing (Redis, BullMQ, Pub/Sub)
- PostgreSQL schema design & transaction safety
- Event-driven systems
- Containerized production environments

---

## Core Expertise

### Backend Architecture
- NestJS 10, Fastify
- Clean modular structure
- RBAC & multi-tenant isolation
- JWT auth (access + refresh flow)
- RESTful APIs with strict validation

### Data & Consistency
- PostgreSQL 16 (ACID, indexing, constraints)
- Prisma & TypeORM
- Monetary precision using integer storage
- DB-level transactional guarantees
- Soft deletes & audit-friendly schemas

### Asynchronous & Real-Time Systems
- Redis 7
- BullMQ producer-consumer patterns
- Redis Pub/Sub for cross-service communication
- WebSocket streaming
- Background workers separated from API lifecycle

### Infrastructure & Tooling
- Docker & Docker Compose
- Monorepo architecture (Turborepo + pnpm workspaces)
- Strict TypeScript (v5)
- Environment-based config
- Migration-based database versioning

---

# Flagship Projects

---

## 💊 MedShop — Multi-Tenant Medical Shop SaaS

A production-grade B2B SaaS platform built for small medical shops in India.

**Architecture Highlights:**

- Row-level multi-tenancy using `shop_id` isolation across guards, services, and queries  
- RBAC with OWNER / MANAGER / STAFF roles  
- Atomic stock deduction using DB transactions  
- FEFO batch handling (First Expiry First Out)  
- All money stored in paise (integer-based accounting to avoid float errors)  
- JWT-based auth with rotating refresh tokens  
- Redis-backed background processing  
- Fully containerized local and production setup  

**Tech Stack:**  
NestJS 10 · PostgreSQL 16 · Redis 7 · BullMQ · Next.js 14 · TypeScript (strict mode)

This project reflects production-oriented thinking: data integrity first, concurrency-safe inventory logic, and maintainable service boundaries.

---

## ⚡ Order Execution Engine — Async Distributed Processing System

A high-performance order execution backend built with Fastify and Redis-based worker architecture.

**Architecture Highlights:**

- Producer–consumer model using BullMQ  
- Orders queued instantly; workers process independently  
- API remains responsive under load  
- Redis Pub/Sub bridges worker and WebSocket server  
- Real-time order status streaming  
- Strategy pattern for smart DEX routing  
- Concurrent price discovery using `Promise.all`  
- ACID-compliant order state management in PostgreSQL  

**Tech Stack:**  
Fastify · PostgreSQL · Prisma · Zod · Redis · BullMQ · TypeScript

This system demonstrates async system design, service separation, and real-time event-driven communication.

---

## Engineering Principles

- Design for scale before optimizing prematurely  
- Transactions protect business logic  
- Validation happens at system boundaries  
- Data models determine system quality  
- Services should fail safely and observably  
- Asynchronous processing reduces coupling and improves resilience  

---

## Currently Studying

- Advanced system design patterns  
- Distributed consistency models  
- Scalable database architecture  
- High-performance API design  

---

## Contact

- Email: shivamkr7822@gmail.com  
- LinkedIn: https://www.linkedin.com/in/shivam-kr-chaudhary/  

---

> I am focused on building backend systems that survive real-world usage.
