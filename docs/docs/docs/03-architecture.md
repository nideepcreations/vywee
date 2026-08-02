---
Project: Vywee
Document: System Architecture
Version: 1.0.0
Status: Active
Owner: Product Team
---

# System Architecture

## Objective

Build Vywee as a scalable platform that supports millions of products, users and searches without requiring a major redesign.

---

# High-Level Architecture

```
                  Website
                     │
             Mobile Application
                     │
          ------------------------
                     │
                Backend API
                     │
        -------------------------
        │           │           │
    AI Engine   Database    Storage
```

---

# Frontend

Technology

- Next.js
- React
- TypeScript
- Tailwind CSS
- shadcn/ui
- Framer Motion

Responsibilities

- UI
- Search
- Product Pages
- Compare
- Buying Guides
- Authentication
- My Research

---

# Mobile App

Technology

- React Native
- Expo

Responsibilities

- Search
- Product Pages
- Compare
- In-Store Assistant
- My Research

---

# Backend

Technology

- NestJS
- TypeScript

Responsibilities

- Authentication
- Business Logic
- AI Integration
- Search
- Offers
- Import Engine
- Analytics

---

# Database

Technology

PostgreSQL

Provider

Supabase

Stores

- Products
- Categories
- Brands
- Users
- Research
- Offers
- Price History
- AI Content

---

# Storage

Supabase Storage

Stores

- Images
- Documents
- Generated Assets

---

# AI Layer

Responsibilities

- AI Search
- Product Summary
- Buying Guides
- Comparisons
- SEO
- Recommendations

AI should always work through one internal service.

Never call AI directly from the frontend.

---

# Search Engine

Supports

- Natural Language
- Category Search
- Brand Search
- Budget Search

Future

- Semantic Search
- Voice Search

---

# Import Engine

Supports

- Product URL
- Search URL
- Category URL
- Brand URL
- CSV Import

Imported products remain in Draft until approved.

---

# Security

- HTTPS
- JWT Authentication
- Role Based Access
- Rate Limiting
- Input Validation

---

# Performance Goals

Homepage

<2 seconds

Search

<800 ms

Product Page

<300 ms

Compare

<500 ms

---

# Deployment

Frontend

Vercel

Backend

Railway

Database

Supabase

CDN

Cloudflare

---

# Folder Structure

```
apps/
    web/
    mobile/
    studio/

backend/

packages/

docs/

assets/
```

---

# Architecture Principles

- Mobile First
- API First
- Modular Design
- Reusable Components
- Feature-based Structure
- Separation of Concerns
- AI Ready
- SEO Friendly

---

# Future Scalability

The architecture must support future expansion into:

- Finance
- Insurance
- Travel
- Education
- Digital Services

without redesigning the core platform.

---

# Version History

## 1.0.0

Initial Architecture Document
