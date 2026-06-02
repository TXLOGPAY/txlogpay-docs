TXLOGPAY — Engineering Onboarding

Overview

TXLOGPAY is an operational trade finance infrastructure designed to orchestrate international settlements through operational triggers.

The platform combines:

- operational workflow management
- treasury orchestration
- protected payment lifecycle
- programmable settlement
- multicurrency normalization
- operational event simulation
- distributed settlement infrastructure

The current implementation was intentionally designed as:

- a hackathon MVP
- an enterprise-oriented operational platform
- a programmable settlement proof-of-concept

while preserving:

- modularity
- scalability
- infrastructure abstraction
- invisible blockchain principles

---

Core Philosophy

TXLOGPAY was intentionally built around the concept of:

"Operational events becoming programmable financial triggers."

The platform is NOT:

- a crypto wallet
- a DeFi application
- a token trading platform
- a blockchain-first product

The platform IS:

- operational finance infrastructure
- programmable trade finance infrastructure
- operational treasury orchestration
- event-driven settlement infrastructure

Blockchain operates only as:

- settlement rail
- audit layer
- traceability infrastructure
- programmable execution backend

The user should never need to:

- manage wallets
- understand blockchain
- interact with cryptographic concepts
- handle smart contract complexity

This architectural principle is referred internally as:

"Invisible Blockchain Infrastructure"

---

High-Level Architecture

Current Architecture

Frontend (React + TypeScript)
        ↓
State Management (Zustand)
        ↓
Service Layer
        ↓
Operational Engine
        ↓
Settlement Engine
        ↓
Stellar Testnet

---

Main Infrastructure Layers

1. Frontend Layer

Responsible for:

- operational UX
- dashboard rendering
- forms
- operational timelines
- status monitoring
- simulator controls
- settlement visibility

Main technologies:

- React
- TypeScript
- TailwindCSS
- TanStack Router

---

2. State Layer

Responsible for:

- operational state persistence
- dashboard synchronization
- active operation state
- simulator progression
- financial aggregation

Main technology:

- Zustand

The state layer was intentionally separated from UI rendering to:

- improve maintainability
- simplify business logic orchestration
- reduce component coupling

---

3. Service Layer

This is effectively the operational core of the platform.

Responsible for:

- fee calculation
- multicurrency normalization
- operational triggers
- settlement orchestration
- Stellar integration
- escrow simulation
- event orchestration

Key architectural principle:

- UI should remain lightweight
- operational intelligence should live in services

---

4. Domain Layer

Responsible for:

- operational entities
- business models
- type contracts
- operational enums
- domain consistency

Examples:

- operation
- escrow
- settlement
- operation status

This layer centralizes the platform's operational language.

---

5. Mock Infrastructure Layer

Responsible for:

- simulated APIs
- hackathon operational simulation
- fake institutional integrations

Examples:

- Siscomex simulator
- escrow mock
- anchor simulation

This layer was intentionally isolated to allow future replacement by real institutional integrations.

---

6. Settlement Layer

Responsible for:

- settlement orchestration
- transaction generation
- settlement references
- blockchain interaction
- explorer integration

Current implementation:

- Stellar Testnet

Current purpose:

- architecture validation
- operational demonstration
- programmable settlement proof

---

Repository Structure

Main Structure

src/
supabase/
public/
scripts/

---

src/

Contains the entire application frontend and operational orchestration logic.

Main folders:

src/components
src/pages
src/services
src/stores
src/hooks
src/domain
src/mocks
src/lib
src/integrations
src/routes

---

Architectural Principle

The project intentionally separates:

UX Layer

Responsible for:

- rendering
- interaction
- operational visualization

FROM:

Operational Intelligence Layer

Responsible for:

- calculations
- triggers
- financial orchestration
- settlement logic
- operational progression

This separation significantly improves:

- maintainability
- scalability
- future API integration
- testing capability
- enterprise evolution

---

Operational Lifecycle

The platform currently operates around the following lifecycle:

Operation Created
↓
Guarantee Awaiting Deposit
↓
Payment Proof Uploaded
↓
Guarantee Validated
↓
Operational Monitoring
↓
Operational Trigger Progression
↓
Settlement Execution
↓
Operation Completed

---

Operational Trigger Model

One of the core concepts of TXLOGPAY is:

- settlement conditioned by operational events

Operational events currently simulated:

CREATED
EXPORTER_ACCEPTED
CARGO_SHIPPED
IN_TRANSIT
CUSTOMS_ARRIVAL
CUSTOMS_RELEASED

Each operational milestone may:

- unlock settlement
- advance operational state
- trigger treasury execution

This is effectively:

- event-driven finance infrastructure

---

Current MVP Boundaries

The current MVP intentionally mixes:

- real infrastructure
- simulated integrations

This was a strategic decision to:

- accelerate hackathon delivery
- validate architecture
- preserve scalability potential

---

Real Components

Currently real:

- frontend
- Supabase persistence
- operational workflow
- multicurrency calculations
- fee engine
- Stellar Testnet integration
- settlement references
- operational timeline
- dashboard aggregation

---

Simulated Components

Currently simulated:

- Siscomex
- escrow institution
- fiat banking rails
- off-ramp providers
- anchor providers
- compliance systems
- logistics APIs

The architecture was intentionally designed so these modules can later be replaced without rebuilding the frontend experience.

---

Technical Positioning

Internally, TXLOGPAY should be understood as:

Operational Settlement Orchestration Infrastructure

rather than:

- blockchain app
- wallet product
- crypto interface

This distinction is fundamental to understanding:

- the UX decisions
- the service architecture
- the operational model
- the infrastructure abstraction strategy
