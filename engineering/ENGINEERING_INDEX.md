TXLOGPAY — Engineering Documentation Index

Core Documentation

Document| Purpose
ARCHITECTURE.md| High-level architecture overview
INFRASTRUCTURE_VISION.md| Long-term infrastructure vision
BUSINESS_MODEL.md| Business and monetization strategy
PRICING.md| Operational pricing strategy
FINANCIAL_MODEL.md| Treasury and financial modeling
ROADMAP.md| Product and infrastructure roadmap
SECURITY.md| Security principles and architecture
WHITEPAPER.md| Strategic platform vision
HACKATHON_IMPLEMENTATION.md| Hackathon-specific implementation details

---

Engineering Documentation

Document| Purpose
TXLOGPAY_ENGINEERING_ONBOARDING.md| Complete technical onboarding
TXLOGPAY_ENGINEERING_SUMMARY.md| Executive technical summary
CONTRIBUTING.md| Contribution guidelines
CODE_OF_CONDUCT.md| Community and collaboration standards

---

Portuguese Documentation

Document| Purpose
EXECUTIVE_SUMMARY_PTBR.md| Executive overview in Portuguese
HACKATHON_OVERVIEW_PTBR.md| Hackathon architecture and implementation overview
PITCH_NOTES_PTBR.md| Internal pitch narrative and presentation guidance

---

Visual Assets

Screenshots

docs/screenshots/

Includes:

- dashboard views
- timeline flows
- multicurrency screens
- settlement flows
- operational lifecycle
- landing page

---

Diagrams

docs/diagrams/

Includes:

- architecture diagrams
- settlement flows
- treasury flows
- multicurrency normalization diagrams
- operational lifecycle diagrams

---

Main Architectural Concepts

Invisible Blockchain

Blockchain acts as:

- infrastructure
- settlement rail
- audit layer

NOT:

- user experience

---

Event-Driven Finance

Operational events control:

- treasury progression
- settlement release
- operational lifecycle

---

Treasury Separation

The architecture separates:

- protected operational capital
- platform revenue

---

Operational-First UX

The product prioritizes:

- operational clarity
- treasury visibility
- enterprise experience

NOT:

- crypto-native interaction

---

Main Technology Stack

Frontend:
React
TypeScript
TailwindCSS

State:
Zustand

Backend:
Supabase

Settlement:
Stellar Testnet

Infrastructure:
Cloudflare
Vite

---

Recommended Reading Order

For Business / Product

1. EXECUTIVE_SUMMARY_PTBR.md
2. WHITEPAPER.md
3. BUSINESS_MODEL.md
4. PRICING.md

---

For Engineers

1. TXLOGPAY_ENGINEERING_SUMMARY.md
2. TXLOGPAY_ENGINEERING_ONBOARDING.md
3. ARCHITECTURE.md
4. INFRASTRUCTURE_VISION.md

---

For Hackathon Judges

1. HACKATHON_OVERVIEW_PTBR.md
2. EXECUTIVE_SUMMARY_PTBR.md
3. PITCH_NOTES_PTBR.md

---

Final Engineering Principle

Operational workflow is the product.
Blockchain is infrastructure.
