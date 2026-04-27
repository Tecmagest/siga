# SIGA — Integrated Academic Management System | SUGEST - Unified Management and Education System

## 📌 Overview

SIGA (SUGEST) is an **Integrated Academic Management System** platform designed to centralize and automate educational operations across single or multiple institutions.

The platform integrates:

- Academic management (students, teachers, classes)
- Curriculum and evaluation systems
- Enrollment and registration workflows
- Financial module (tuition/billing)
- Reporting and analytics
- Multi-tenant institutional configuration
- Modern web interface (SPA + PWA)

👉 Backend architecture: :contentReference[oaicite:4]{index=4}  
👉 Frontend architecture: :contentReference[oaicite:5]{index=5}  

---

## 🧠 Integrated System Concept

Unlike fragmented systems, SIGA was designed as a unified platform where:

- Academic, administrative, and financial data are interconnected  
- Processes are automated end-to-end  
- No data duplication occurs  
- Consistency is enforced across all modules  

---

## 🏗️ System Architecture

### Backend
- Clean Architecture (4 layers)
- CQRS + Vertical Slice
- Native multi-tenancy
- Versioned REST API

### Frontend
- Angular 21 (standalone + signals)
- Static SPA (no Node.js in production)
- PWA with offline support
- Feature-based structure (aligned with API)

👉 Details: :contentReference[oaicite:6]{index=6}  

---

## 🔗 Backend–Frontend Integration

- Strong contract using `OperationResult<T>` and `PagedResponse<T>`
- Typed models mirrored on frontend
- Interceptors handle authentication and errors
- Guards enforce role-based access

---

## 🧩 Multi-Tenancy (SaaS-ready)

- Tenant isolation via `InstitutionId`
- JWT-based tenant context
- Visual theming per institution
- Multi-school support in a single instance

---

## ⚙️ System Modules

- Students
- Teachers
- Courses & subjects
- Enrollments & registrations
- Evaluations & grading
- Tuition & billing
- Scheduling & attendance
- Documents & certificates
- Notifications
- Reporting
- Institutional configuration

---

## 🔄 Integrated Workflow Example

### Enrollment → Academic → Financial

1. Student enrollment  
2. Automatic subject registration  
3. Curriculum linkage  
4. Automatic tuition generation  
5. Evaluation feeds reporting  

👉 Fully integrated flow (no redundancy)

---

## 🔐 Security

- JWT + Refresh Tokens
- Role-Based Access Control (RBAC)
- Frontend guards + backend policies
- Tenant-level isolation

---

## 📊 Scale & Complexity

- ~76,000 lines of code
- 233 HTTP endpoints
- 1200+ automated tests
- 60 domain entities

👉 Source: :contentReference[oaicite:7]{index=7}  

---

## 🧠 Technical Highlights

- Modular architecture (Vertical Slice)
- True multi-tenancy (not simulated)
- Offline-capable frontend (PWA)
- Highly configurable system
- Full domain integration

---

## 🚀 Tech Stack

### Backend
- .NET 10
- EF Core
- PostgreSQL
- JWT

### Frontend
- Angular 21
- Angular Material (M3)
- Tailwind CSS
- Service Worker (PWA)

---

## 📈 Project Level

This is not a simple CRUD system.

It is a:
- Multi-tenant platform
- Integrated academic + financial system
- Scalable enterprise-grade solution

---

## 📄 License

Private project — sanitized version for technical demonstration.
