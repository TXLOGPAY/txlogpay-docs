Part 2 — Frontend Structure, Routes and UI Architecture

Frontend Overview

The frontend was designed as:

- enterprise-oriented operational software
- operational dashboard infrastructure
- financial workflow management interface

The UX intentionally avoids:

- crypto-native terminology
- wallet-first interaction
- blockchain-centric flows

The interface prioritizes:

- operational monitoring
- payment protection
- treasury visibility
- workflow progression
- event-driven status tracking

---

Frontend Stack

Core Technologies

React
TypeScript
Vite
TailwindCSS
TanStack Router
Zustand

---

Why This Stack Was Chosen

React

Chosen for:

- modularity
- component scalability
- ecosystem maturity
- rapid UI iteration

---

TypeScript

Chosen for:

- operational consistency
- safer domain modeling
- typed services
- predictable financial calculations

The project relies heavily on:

- operational entities
- financial state
- multicurrency calculations
- event orchestration

Strong typing became essential.

---

TailwindCSS

Chosen for:

- fast UI iteration
- enterprise dark-mode consistency
- low CSS overhead
- component flexibility

The visual language intentionally resembles:

- operational banking systems
- treasury dashboards
- institutional financial software

---

TanStack Router

Responsible for:

- route organization
- nested operational pages
- operational detail navigation
- parameterized operation flows

This allowed the platform to evolve toward:

- modular operational workflows
- scalable routing architecture

---

Routing Structure

Main Routing Philosophy

Routes were separated according to:

- operational lifecycle
- operational detail depth
- settlement progression

Examples:

/operacoes
/operacoes/:id
/operacoes/:id/pagamento

This structure allows:

- isolated operational visualization
- lifecycle segmentation
- modular settlement pages

---

Main Pages

Dashboard

Main objective:

- operational overview
- financial visibility
- protected payment aggregation
- operation monitoring

Key responsibilities:

- render KPI cards
- display multicurrency totals
- show operational metrics
- summarize active operations

The dashboard acts as:

- treasury control center
- operational cockpit

---

Operations List

Main objective:

- centralized operation monitoring

Responsibilities:

- list operations
- display statuses
- show protected values
- show currencies
- allow operational drill-down

This page acts as:

- operational command center

---

Operation Details Page

One of the most important architectural pages.

Responsibilities:

- operational timeline
- guarantee lifecycle
- simulator progression
- settlement progression
- operational state transitions

This page centralizes:

- operational orchestration
- treasury visibility
- event-driven settlement logic

---

Landing Page

Main objective:

- explain the platform
- demonstrate value proposition
- simulate institutional positioning
- onboard potential users

Key components:

- hero section
- pricing comparison
- calculator
- operational flow explanation

This page was intentionally designed to resemble:

- enterprise fintech products
- institutional SaaS platforms

---

UI Component Architecture

components/

Contains:

- reusable UI logic
- operational rendering blocks
- dashboard widgets
- timeline infrastructure
- financial cards

The component layer intentionally avoids:

- business calculations
- settlement logic
- heavy operational orchestration

Business intelligence should remain inside:

- services
- stores
- domain models

---

Key UI Components

Timeline Component

One of the most important components in the project.

Responsibilities:

- display operational progression
- render operational milestones
- show settlement progression
- display operational state

The timeline acts as:

- operational audit trail
- visual workflow engine

---

Financial Cards

Responsibilities:

- treasury visualization
- multicurrency aggregation
- protected payment visibility
- operational metrics

The financial cards intentionally centralize:

- treasury clarity
- operational awareness
- enterprise dashboard feeling

---

Guarantee Upload Component

Responsibilities:

- payment proof upload
- operational validation trigger
- guarantee lifecycle progression

This component acts as:

- bridge between operational workflow and treasury progression

---

Simulator Component

Responsibilities:

- simulate operational events
- advance operational statuses
- trigger settlement progression

The simulator demonstrates:

- event-driven financial orchestration

without requiring:

- real institutional APIs

---

Settlement Components

Responsibilities:

- show settlement execution
- render blockchain references
- display settlement confirmation
- provide audit visibility

The UX intentionally avoids:

- crypto-native complexity
- wallet interaction
- blockchain jargon

---

UI Philosophy

The UI was intentionally designed around:

Enterprise Operational Simplicity

This means:

- low cognitive friction
- operational clarity
- treasury visibility
- progressive disclosure

The interface should feel:

- institutional
- operational
- financial
- trustworthy

NOT:

- speculative
- crypto-native
- retail blockchain

---

Dark Theme Strategy

The dark institutional theme was intentionally chosen to resemble:

- treasury systems
- trading infrastructure
- operational banking software
- enterprise financial dashboards

This significantly improved:

- perceived maturity
- institutional positioning
- enterprise UX feeling

---

UX Abstraction Strategy

One of the strongest architectural principles of the frontend:

Hide infrastructure complexity.
Expose operational clarity.

The user should understand:

- operations
- guarantees
- status progression
- payment lifecycle

without needing to understand:

- blockchain
- wallets
- settlement rails
- distributed ledgers

---

State Management Philosophy

The frontend intentionally separates:

- rendering
- operational intelligence
- persistence
- orchestration

This prevents:

- component overload
- duplicated business logic
- operational inconsistency

The architecture already resembles:

- scalable enterprise frontend systems

rather than:

- simple hackathon frontend structure

---

Current UX Strengths

Current strong points:

- operational clarity
- timeline visualization
- treasury abstraction
- enterprise positioning
- multicurrency visibility
- settlement storytelling

---

Current UX Technical Debt

Still pending:

- responsive optimization
- loading state standardization
- error boundary standardization
- permission abstraction
- audit visualization
- role segregation
- institutional onboarding flows

These items belong primarily to:

- beta phase
- production evolution
