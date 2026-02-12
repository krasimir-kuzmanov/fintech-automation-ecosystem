# 💳 FinTech Automation Ecosystem

A complete full-stack automation ecosystem built around a sample fintech application.

This portfolio demonstrates clean automation architecture, separation of concerns between UI and API testing, and end-to-end system consistency validation.

---

# 🏗 System Architecture

Frontend (React + Vite)  
⬇  
Backend (Spring Boot, Java 21)  
⬇  
H2 In-Memory Database  

Automation Layers:

- API Test Suite (RestAssured + JUnit 5)
- UI Test Suite (Selenide + JUnit 5)
- UI ↔ API cross-layer consistency validation
- CI pipelines per project

---

# 🔧 Application Repositories

## Backend — `fintech-backend`

Spring Boot application providing:

- JWT authentication
- User registration & login
- Account funding
- Payment processing
- Transaction history
- Deterministic `/test/reset` endpoint for reliable automation

🔗 https://github.com/krasimir-kuzmanov/fintech-backend

---

## Frontend — `fintech-frontend`

React application providing:

- Login / Register flows
- Fund account
- Make payment
- Transaction history
- Logout with route protection
- Stable `data-testid` selectors for automation

🔗 https://github.com/krasimir-kuzmanov/fintech-frontend

---

# 🧪 Automation Repositories

## API Test Suite — `fintech-api-tests`

![API Tests](https://github.com/krasimir-kuzmanov/fintech-api-tests/actions/workflows/api-tests.yml/badge.svg)

- Full endpoint coverage
- Negative validation scenarios
- Security tests (401 / 403)
- Deterministic execution via `/test/reset`
- Clean client-based architecture
- GitHub Actions CI

🔗 https://github.com/krasimir-kuzmanov/fintech-api-tests

---

## UI Test Suite — `fintech-ui-tests`

![UI Tests](https://github.com/krasimir-kuzmanov/fintech-ui-tests/actions/workflows/ui-tests.yml/badge.svg)

- Selenide + JUnit 5
- Page Object Model
- Chrome execution
- API-assisted setup for deterministic state
- UI ↔ API transaction ID consistency validation
- Multiple payment verification
- GitHub Actions CI starting backend + frontend

🔗 https://github.com/krasimir-kuzmanov/fintech-ui-tests

---

# 🎯 What This Demonstrates

- Senior-level automation architecture thinking
- Full-stack system understanding
- Clear separation of UI and API test responsibilities
- Deterministic test setup
- Cross-layer consistency validation
- CI/CD integration
- Production-style project structure

---

# 📌 Design Philosophy

- Small, high-signal test suites
- No unnecessary duplication between UI and API layers
- API used for setup and cross-verification in UI tests
- Clean architecture over test volume
- Deterministic and reproducible execution

---

This ecosystem is intentionally designed to simulate a realistic automation strategy for a fintech product.
