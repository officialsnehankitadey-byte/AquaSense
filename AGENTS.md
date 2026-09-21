# AquaSense — AI-Driven Water Network Intelligence

## Overview
AquaSense is an AI-driven water network intelligence platform designed for real-time monitoring, anomaly detection, leak localization, and repair prioritization.

**Core Flow:**
Sense → Detect → Localize → Prioritize Repair → Verify

---

## Team Structure & Ownership
AquaSense is built by a 2-person team during a hackathon.

### Repository Structure
- `frontend/` — Frontend UI / dashboard owned primarily by **Member 1**
- `backend/` — Backend logic, AI models, and data ingestion owned primarily by **Member 2**
- `docs/` — Shared documentation
- `AGENTS.md` — Shared AI coding rules and team instructions

### Member 1 — Frontend Responsibilities
- Next.js / React / TypeScript / Tailwind CSS
- Dashboard UI
- Network visualization
- Sensor status indicators
- Incident UI & alerts
- Charts and metrics displays
- Responsive web design
- Frontend API integration
- Frontend testing

### Member 2 — Backend/AI Responsibilities
- Python / FastAPI
- Sensor simulation & data ingestion
- Database management & schemas
- Anomaly detection models
- Leak localization algorithms
- Incident prioritization engine
- Water-saved metric calculations
- Backend REST APIs
- Backend testing

### Shared Responsibilities
- API contract design & alignment
- System integration
- End-to-end testing
- Documentation & architecture guides
- Deployment setup
- Final demo preparation and bug fixing

---

## AI Coding Rules
All AI agents working on this repository MUST strictly follow these rules:

1. **Inspect Before Modifying**: Always inspect existing code before making modifications.
2. **Task Scoping**: Keep changes strictly scoped to the requested task.
3. **Respect Ownership**: Do not modify the other teammate's area unless explicitly asked.
4. **Preserve Working Code**: Do not rewrite working code unnecessarily.
5. **Minimal Dependencies**: Do not add unnecessary external libraries or dependencies.
6. **Functionality Preservation**: Preserve existing working functionality across all changes.
7. **Type Safety & Structure**: Use strong TypeScript types and clear component structure on the frontend.
8. **Predictable APIs**: Keep backend APIs clean, documented, and predictable.
9. **Mock Data Separation**: Use mock data only where explicitly appropriate, and clearly separate mock data from real API data.
10. **Scope Guardrails**: Never add authentication, payment processing, or unrelated feature bloat unless explicitly requested.
11. **Pre-flight Verification**: Before completing a task, check for syntax/lint errors and verify that existing functionality still works.
12. **Strict Scope Control**: Do not make extra changes outside the requested scope just because they seem useful.

---

## Git Workflow
- `main`: Stable release branch.
- `develop`: Primary integration branch.
- `feature/*`: Individual feature work branches.

### Workflow Guidelines
- **Never develop directly on `main` or `develop`.** Always branch off to `feature/*`.
- Keep commits small, descriptive, and atomic. Do not create fake commits.
- Pull/rebase from `develop` before starting major integration work when appropriate.
- Feature branches merge into `develop` through PR or review.
- `develop` is merged into `main` for stable releases.

---

## Frontend / Backend Integration
- **API First**: Agree on API contracts and response schemas before implementation.
- **Mocking**: Frontend may initially use clearly marked mock data while backend APIs are in development.
- **Contract Stability**: Do not silently change API response formats that the other side depends on.
- **Documentation**: Keep API endpoints, request payloads, and response schemas documented.
- **Backward Compatibility**: Prefer backward-compatible API revisions whenever possible.
