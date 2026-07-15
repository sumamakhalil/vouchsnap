# VouchSnap

![React](https://img.shields.io/badge/React-18-61DAFB?logo=react)
![Vite](https://img.shields.io/badge/Vite-5-646CFF?logo=vite)
![Node.js](https://img.shields.io/badge/Node.js-Express-339933?logo=node.js)
![Supabase](https://img.shields.io/badge/Supabase-PostgreSQL-3ECF8E?logo=supabase)
![Gemini](https://img.shields.io/badge/Google-Gemini_AI-4285F4?logo=google)
![License](https://img.shields.io/badge/License-MIT-blue)

An AI-powered SaaS platform that helps freelancers, agencies, and businesses collect, manage, polish, and showcase client testimonials through AI-assisted workflows, embeddable widgets, and social media exports.

## Table of Contents

- [Overview](#overview)
- [Live Demo](#live-demo)
- [Screenshots](#screenshots)
- [System Architecture](#system-architecture)
- [Tech Stack](#tech-stack)
- [Key Features](#key-features)
- [Engineering Highlights](#engineering-highlights)
- [Technical Challenges](#technical-challenges)
- [What I Learned](#what-i-learned)
- [Future Improvements](#future-improvements)
- [Contact](#contact)

## Overview

VouchSnap is a modern AI-powered SaaS platform designed to help freelancers, agencies, and businesses effortlessly collect, manage, and showcase client testimonials.

Instead of manually requesting reviews and formatting them for marketing, VouchSnap automates the entire workflow—from collecting feedback through a public link to polishing testimonials with AI, exporting branded social media graphics, and embedding testimonials directly into websites.

The platform follows a production-ready SaaS architecture with secure authentication, subscription management, role-based access, AI integration, and scalable cloud infrastructure.

---

## Live Demo

**Coming Soon**

---

## Screenshots

### Dashboard

![Dashboard](assets/dashboard.png)

## System Architecture

```mermaid
flowchart TD

A[Client Browser]

subgraph Frontend
B[React + Vite]
C[Dashboard]
D[Testimonial Collection]
E[LinkedIn Export]
end

subgraph Backend
F[Express.js API]
G[Authentication]
H[Business Logic]
I[Subscription Management]
end

subgraph Database
J[(Supabase PostgreSQL)]
K[Supabase Storage]
end

subgraph AI
L[Google Gemini API]
end

subgraph Payments
M[Lemon Squeezy]
end

A --> B
B --> C
B --> D
B --> E

B --> F

F --> G
F --> H
F --> I

G --> J
H --> J
H --> K

H --> L

I --> M

J --> B
K --> B
```

### Architecture Diagram

![Architecture](assets/architecture.png)
