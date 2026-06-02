Part 10 — Developer Onboarding, Local Environment and Final Engineering Mental Model

Developer Onboarding Overview

This section explains:

- how a new developer should think about TXLOGPAY
- how the local environment works
- where to start
- which files matter most
- how the architecture should evolve

This is arguably:

- the most important onboarding section

because understanding TXLOGPAY is less about:

- reading components

and more about:

- understanding the operational philosophy

---

The Most Important Concept

Before touching the codebase, every developer must understand:

TXLOGPAY is NOT a blockchain product.

TXLOGPAY is:

- operational finance infrastructure
- trade finance orchestration infrastructure
- treasury workflow infrastructure
- programmable operational settlement infrastructure

Blockchain is:

- infrastructure
  NOT:
- user experience

This distinction influences:

- architecture
- UX
- services
- settlement
- terminology
- product decisions

---

How Developers Should Think About The Platform

The correct mental model is:

Operational Workflow
↓
Treasury Logic
↓
Settlement Orchestration
↓
Blockchain Infrastructure

NOT:

Blockchain
↓
Frontend

This distinction is critical.

---

Current Architectural Priorities

The current architecture prioritizes:

1. Operational Clarity

The user must understand:

- operations
- guarantees
- progression
- settlement lifecycle

without understanding:

- blockchain

---

2. Treasury Visibility

The platform must preserve:

- protected value clarity
- fee separation
- operational transparency

---

3. Infrastructure Abstraction

Institutional infrastructure should remain:

- replaceable
- modular
- isolated

---

4. Enterprise UX

The product should resemble:

- treasury software
- operational banking software
- institutional infrastructure

NOT:

- crypto applications

---

Local Development Overview

Current local stack:

Node.js
Vite
React
Supabase
TailwindCSS

---

Main Local Responsibilities

The local environment currently handles:

- frontend rendering
- operational orchestration
- mock infrastructure
- Stellar testnet interaction
- dashboard aggregation
- operational workflows

---

Important Folders For New Developers

src/services

START HERE FIRST.

This folder explains:

- how the platform thinks
- how treasury behaves
- how settlement works
- how operations progress

This is effectively:

- the operational brain

---

src/domain

Read second.

This folder explains:

- business entities
- operational meaning
- lifecycle structure
- operational contracts

This folder teaches:

- the language of TXLOGPAY

---

src/mocks

Read third.

This folder explains:

- which integrations are simulated
- how infrastructure abstraction works
- how the MVP emulates institutional systems

This folder is critical for understanding:

- the hackathon strategy

---

src/lib

Important for:

- financial calculations
- multicurrency logic
- fee modeling
- formatting helpers

One of the most important files:

financial-calculations.ts

This file contains:

- the economic behavior of the platform

---

src/components

Read AFTER understanding services.

Components are intentionally:

- lightweight
- rendering-focused
- operationally visual

Avoid placing:

- treasury logic
- settlement orchestration
- financial calculations

inside components.

---

src/routes

Important for understanding:

- operational navigation
- lifecycle segmentation
- operational page hierarchy

---

src/stores

Important for understanding:

- operational persistence
- UI synchronization
- global operational state

---

Operational Flow Every Developer Must Understand

Core lifecycle:

Operation Created
↓
Guarantee Pending
↓
Proof Uploaded
↓
Guarantee Validated
↓
Operational Monitoring
↓
Simulator Progression
↓
Trigger Match
↓
Settlement Execution
↓
Operation Completed

This flow drives:

- UI
- services
- dashboard
- treasury logic
- settlement orchestration

---

Most Important Architectural Layers

1. Operational Layer

Represents:

- business workflows
- operational lifecycle
- logistics progression

---

2. Treasury Layer

Represents:

- protected capital
- fee separation
- conditional release

---

3. Settlement Layer

Represents:

- Stellar interaction
- settlement confirmation
- transaction references

---

4. Infrastructure Layer

Represents:

- mocks
- future integrations
- API abstraction

---

Current MVP Philosophy

The MVP intentionally validates:

Operational orchestration first.
Institutional integration later.

This was:

- strategically correct
- execution-efficient

---

What New Developers Should Avoid

Avoid:

- exposing blockchain terminology in UX
- adding wallet-centric flows
- leaking infrastructure complexity
- mixing financial logic into components
- bypassing services layer
- hardcoding operational states

---

Most Important UX Principle

The UX should always prioritize:

Operational simplicity.

The platform should feel:

- institutional
- operational
- trustworthy
- financial

NOT:

- speculative
- crypto-native
- blockchain-first

---

How To Think About Future Integrations

Current integrations are mostly:

- simulated

Future architecture should replace:

- mocks
  with:
- providers

WITHOUT rebuilding:

- operational flows
- UI
- lifecycle logic

This is extremely important.

---

Most Important Future Production Layers

Future production evolution will likely require:

Treasury Ledger

For:

- reconciliation
- reserve tracking
- settlement balancing

---

Anchor Integration

For:

- fiat interoperability
- banking rails
- off-ramp infrastructure

---

Compliance Infrastructure

For:

- KYC
- AML
- transaction monitoring

---

Observability

For:

- telemetry
- infrastructure tracing
- operational monitoring

---

Current Architectural Strengths

The strongest architectural aspects today are:

1. Operational-first thinking

---

2. Treasury separation

---

3. Event-driven settlement logic

---

4. Infrastructure abstraction

---

5. Invisible blockchain philosophy

---

Current Weaknesses

Still pending:

- institutional hardening
- real integrations
- audit infrastructure
- observability
- reconciliation
- production treasury ledger
- robust failure recovery

These are:

- expected
- acceptable for the current stage

---

The Most Important Hidden Innovation

The strongest hidden innovation in TXLOGPAY is NOT:

- Stellar
- blockchain
- settlement rails

The strongest innovation is:

Operationally-aware programmable finance.

Meaning:

- financial execution depends on operational reality

This is:

- conceptually sophisticated
- institutionally relevant
- highly scalable

---

Final Engineering Mental Model

Every developer joining TXLOGPAY should mentally model the platform as:

Operational Workflow Engine
+
Treasury Orchestration Infrastructure
+
Programmable Settlement Layer

NOT:

- crypto application
- wallet interface
- blockchain demo

---

Final Architectural Insight

The most important architectural principle of the entire project is:

The operational workflow is the product.
Blockchain is infrastructure.

This principle defines:

- the UX
- the architecture
- the services
- the treasury logic
- the settlement model
- the future production strategy

and should remain preserved throughout the evolution of the platform.

---

END OF ENGINEERING ONBOARDING
