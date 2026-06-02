Part 4 — Domain Layer, State Management and Operational Modeling

Domain Layer Overview

The domain layer represents:

- the operational language of TXLOGPAY
- the business entities
- the lifecycle contracts
- the operational modeling structure

This layer centralizes:

- operational meaning
- financial semantics
- lifecycle definitions
- status consistency

The domain layer is one of the clearest indicators that the project evolved beyond:

- UI prototyping
- isolated screens
- simple hackathon frontend logic

The platform already behaves conceptually like:

- operational finance software

---

Domain Philosophy

The architecture intentionally separates:

How the system looks

FROM:

How the business behaves

The domain layer defines:

- operational truth
- lifecycle states
- entity structure
- financial meaning

while the frontend merely:

- renders
- interacts
- visualizes

This separation is critical for:

- scalability
- maintainability
- API evolution
- backend migration
- future microservice extraction

---

Main Domain Concepts

The project currently revolves around several core entities:

Operation
Escrow
Settlement
Operational Status
FX Normalization
Guarantee Lifecycle

These entities collectively define:

- the operational model
- the treasury behavior
- the settlement orchestration

---

Operation Entity

The most important entity in the platform.

Represents:

- international trade operation
- protected payment workflow
- operational settlement lifecycle

An operation contains:

- importer information
- exporter information
- operational value
- currency
- target trigger
- operational progression
- guarantee state
- settlement state

The operation entity effectively acts as:

- the root aggregate of the platform

---

Operation Lifecycle

Current operational lifecycle:

Created
↓
Guarantee Pending
↓
Proof Uploaded
↓
Guarantee Validated
↓
Operational Monitoring
↓
Trigger Achieved
↓
Settlement Processing
↓
Settlement Confirmed
↓
Completed

This lifecycle is fundamental to understanding:

- frontend flows
- service orchestration
- simulator behavior
- treasury progression

---

Operation Status Modeling

One of the strongest architectural decisions.

Operational statuses were intentionally isolated as:

- centralized operational constants
- reusable lifecycle states
- shared orchestration contracts

This prevents:

- duplicated strings
- inconsistent status rendering
- operational divergence

---

Current Operational Events

The simulator currently operates with:

CREATED
EXPORTER_ACCEPTED
CARGO_SHIPPED
IN_TRANSIT
CUSTOMS_ARRIVAL
CUSTOMS_RELEASED

These statuses simulate:

- real-world trade milestones
- logistics progression
- customs advancement
- operational validation

---

Why This Matters

The operational events are not merely:

- UI labels

They effectively act as:

- treasury conditions
- programmable triggers
- settlement gates

This transforms the operational model into:

- event-driven finance infrastructure

---

Settlement Entity

Represents:

- settlement progression
- blockchain execution
- treasury completion

A settlement may contain:

- transaction reference
- settlement status
- confirmation state
- explorer hash
- operational linkage

Current implementation:

- Stellar Testnet references

---

Escrow Entity

Represents:

- protected operational capital
- treasury reservation lifecycle
- guarantee orchestration

The escrow model currently simulates:

- institutional capital protection
- operational reserve management

Even though:

- real banking custody is not yet integrated

the domain modeling already resembles:

- real escrow systems

---

Why The Domain Layer Is Important

Without domain separation:

- operational logic spreads into components
- settlement logic becomes duplicated
- treasury orchestration becomes inconsistent

The current structure already enables:

- future backend extraction
- API centralization
- operational consistency

---

State Management Layer

Zustand Architecture

The project uses:

- Zustand

for:

- operational state orchestration
- lightweight global state
- dashboard synchronization
- operation lifecycle persistence

---

Why Zustand Was A Good Choice

The project does not currently require:

- extremely complex normalized stores
- Redux-level boilerplate
- event sourcing complexity

Zustand provides:

- low overhead
- simplicity
- scalability
- easy operational orchestration

This was a very pragmatic architectural choice.

---

Current Store Responsibilities

The stores currently centralize:

- active operations
- operational status
- settlement progression
- dashboard aggregation
- multicurrency visibility

---

Store Philosophy

The architecture intentionally separates:

Persistent operational state

FROM:

Rendering logic

This improves:

- maintainability
- operational consistency
- lifecycle orchestration

---

Operational Synchronization

One important aspect of the current architecture:

The UI does not independently decide:

- treasury progression
- operational status
- settlement execution

Instead:

- services orchestrate
- stores persist
- UI reflects

This is already very similar to:

- enterprise operational systems

---

Why This Architecture Is Strong

The current structure already enables:

- future websocket integration
- real-time operational monitoring
- multi-user synchronization
- audit visibility
- operational telemetry

without requiring:

- major frontend rewrites

---

Hooks Layer

hooks/

Responsible for:

- reusable frontend orchestration
- operational abstractions
- UI state composition
- lifecycle helpers

The hooks layer helps:

- reduce component complexity
- isolate repetitive operational logic
- improve frontend maintainability

---

Integrations Layer

integrations/

Responsible for:

- external infrastructure abstractions
- API orchestration
- future integration adapters

This layer is strategically important because:

- the current MVP still relies heavily on simulated infrastructure

Future integrations may include:

- banking APIs
- anchor providers
- FX providers
- compliance systems
- customs APIs

The integration layer will become:

- one of the most important production layers

---

lib/ Layer

lib/

Contains:

- shared helpers
- financial calculations
- utility abstractions
- formatting logic
- normalization logic

One particularly important file identified:

financial-calculations.ts

This file centralizes:

- fee logic
- protected amount logic
- treasury calculations
- financial consistency

---

Why This File Matters

This file effectively defines:

- the economic behavior of the platform

It controls:

- operational pricing
- protected value
- treasury separation
- platform revenue logic

This makes it:

- one of the highest business impact files in the entire project

---

Supabase Domain Persistence

The platform currently uses Supabase for:

- operational persistence
- authentication
- storage
- operational lifecycle retention

Current architecture resembles:

- Backend-as-a-Service operational backend

This accelerated:

- MVP delivery
- persistence implementation
- operational storage
- authentication abstraction

---

Storage Usage

Current storage use cases:

- proof upload
- operational documents
- guarantee evidence

The upload architecture already resembles:

- institutional operational systems

---

Architectural Strength Summary

The strongest hidden strengths of the current architecture are:

1. Domain Separation

Operational meaning exists outside UI rendering.

---

2. Service Isolation

Business logic remains centralized.

---

3. Treasury Modeling

Financial behavior already resembles real institutional workflows.

---

4. Event-Driven Thinking

Operational milestones drive financial progression.

---

5. Infrastructure Abstraction

Mocked systems can later be replaced by real providers.

---

Current Domain Technical Debt

Still pending:

- role modeling
- permission segregation
- audit entities
- reconciliation entities
- dispute handling
- retry entities
- settlement recovery flows
- AML/KYC lifecycle modeling

These belong primarily to:

- beta
- production evolution
- institutional readiness

---

Most Important Architectural Insight

The current architecture already demonstrates:

Operational Finance Thinking

rather than:

- simple frontend assembly
- isolated blockchain demo
- basic payment prototype

This is what makes TXLOGPAY significantly more mature than most hackathon projects.
