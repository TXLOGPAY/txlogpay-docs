Part 5 — Supabase Architecture, Persistence Layer and Operational Data Flow

Supabase Overview

Supabase currently acts as:

- operational persistence layer
- authentication provider
- storage infrastructure
- lightweight backend platform

The choice of Supabase was strategic because it allowed:

- rapid MVP delivery
- operational persistence
- authentication abstraction
- file upload infrastructure
- SQL-based scalability

without requiring:

- custom backend infrastructure
- DevOps complexity
- server orchestration

---

Current Role of Supabase

The current architecture uses Supabase for:

Authentication
Database Persistence
File Storage
Operational State Retention

Supabase effectively acts as:

- the operational memory of the platform

---

Why This Architecture Was Smart

The platform focuses heavily on:

- operational workflows
- treasury orchestration
- timeline progression
- multicurrency operations

Using Supabase allowed the team to prioritize:

- operational UX
- settlement orchestration
- business modeling

instead of:

- backend infrastructure engineering

This was a very pragmatic MVP decision.

---

Current Persistence Philosophy

The persistence layer was intentionally designed around:

Operational lifecycle persistence

rather than:

- blockchain-native storage
- on-chain operational state
- decentralized application persistence

The blockchain layer is used only for:

- settlement references
- traceability
- execution proof

Operational truth remains:

- off-chain
- operational
- queryable
- manageable

---

Main Persistence Concepts

The database currently revolves around:

- operations
- statuses
- guarantees
- settlement references
- multicurrency values
- operational events

---

Operations Table

One of the most important persistence entities.

Represents:

- the root operational object
- the trade finance workflow
- the settlement orchestration lifecycle

An operation may contain:

- importer
- exporter
- operation amount
- fee amount
- currency
- target trigger
- operational status
- guarantee status
- settlement status
- proof references
- timestamps

This table effectively acts as:

- the operational backbone of the platform

---

Operational Lifecycle Persistence

The persistence layer stores:

- operational progression
- timeline history
- guarantee lifecycle
- settlement progression

This enables:

- operational reconstruction
- auditability
- operational visibility
- future reporting

---

Guarantee Persistence

The system persists:

- proof uploads
- guarantee state
- validation progression

Current lifecycle:

Awaiting Deposit
↓
Proof Uploaded
↓
Guarantee Validated

This structure already resembles:

- institutional treasury workflows

---

Settlement Persistence

Current settlement persistence stores:

- settlement status
- transaction references
- Stellar hashes
- execution timestamps

Current purpose:

- operational traceability
- settlement auditability
- timeline reconstruction

---

Multicurrency Persistence

The persistence layer stores:

- native operation currency
- operation amount
- normalized reporting logic

The architecture intentionally preserves:

- original operational currency

while enabling:

- treasury normalization
- dashboard aggregation
- financial reporting consistency

---

Important Financial Principle

The platform intentionally preserves:

- operational truth in native currency

Example:

Operation = 1000 CNY

rather than:

- permanently converting operations into USD

Normalization occurs:

- at reporting layer
- dashboard aggregation layer

This is architecturally correct because:

- operational truth remains immutable
- reporting logic remains flexible

---

File Storage Architecture

Supabase storage currently handles:

- payment proofs
- operational attachments
- guarantee evidence

This allows:

- operational auditability
- treasury verification
- proof retention

---

Upload Flow

Current upload lifecycle:

User Upload
↓
Storage Bucket
↓
Operation Association
↓
Timeline Update
↓
Guarantee Progression

This architecture already resembles:

- enterprise document workflows

---

Authentication Layer

Supabase Auth currently provides:

- user authentication
- session management
- access control abstraction

Current MVP scope:

- lightweight authentication

Future production evolution may include:

- RBAC
- enterprise permissions
- treasury segregation
- importer/exporter separation
- auditor roles
- compliance access

---

Current Database Philosophy

The current persistence model intentionally prioritizes:

- operational simplicity
- lifecycle clarity
- MVP scalability

The architecture intentionally avoids:

- premature microservices
- excessive normalization
- overengineered event sourcing

This was a very strong architectural decision for the hackathon phase.

---

Why The Current Persistence Model Works Well

The project currently behaves primarily as:

- operational workflow platform

rather than:

- high-frequency financial engine

This makes:

- relational operational persistence

a very appropriate choice.

---

Supabase Migrations

The project already demonstrates:

- migration thinking
- schema evolution awareness
- operational persistence planning

This significantly improves:

- maintainability
- future onboarding
- infrastructure consistency

---

Current Persistence Strengths

1. Operational Lifecycle Clarity

The database mirrors:

- real operational progression

rather than:

- generic transaction storage

---

2. Treasury Separation

The architecture correctly separates:

- protected amount
- operational fee
- treasury logic

---

3. Multicurrency Awareness

The persistence model preserves:

- native operational currency

while supporting:

- reporting normalization

---

4. Infrastructure Decoupling

Settlement infrastructure remains abstracted from:

- operational persistence

This is extremely important.

---

Current Technical Debt

Still pending:

- audit tables
- operational history tables
- immutable event logs
- reconciliation tables
- retry tracking
- settlement recovery states
- AML/KYC entities
- dispute workflows
- treasury ledger abstraction

These belong primarily to:

- beta phase
- institutional evolution

---

Future Production Persistence Vision

The architecture already supports future evolution toward:

Operational Ledger Infrastructure

Potential future layers:

- treasury ledger
- reconciliation engine
- settlement journal
- audit event store
- compliance tracking
- operational observability

---

Future Infrastructure Possibilities

Possible future integrations:

- PostgreSQL scaling
- event streaming
- Kafka/PubSub
- treasury reconciliation services
- institutional data lakes
- real-time operational telemetry

---

One Of The Most Important Architectural Decisions

The strongest persistence-related decision was:

Keeping blockchain outside operational persistence.

Operational truth remains:

- queryable
- mutable where necessary
- operationally manageable

while blockchain remains:

- settlement evidence
- traceability layer
- immutable reference

This distinction is extremely sophisticated.

---

Why This Architecture Is Mature

Many Web3 projects incorrectly attempt to:

- store operational state on-chain
- make blockchain the application database

TXLOGPAY intentionally avoids this.

Instead:

- blockchain acts as settlement infrastructure
- operational state remains operational

This is much closer to:

- real enterprise financial infrastructure
- institutional treasury systems
- operational banking software

than:

- typical blockchain applications

---

Final Architectural Insight

The Supabase architecture demonstrates:

Operational-first financial infrastructure thinking.

The project was designed around:

- operational workflows
- treasury progression
- settlement orchestration
- financial lifecycle visibility

not around:

- blockchain hype
- token speculation
- crypto-native interaction

This is one of the strongest strategic aspects of the entire architecture.
