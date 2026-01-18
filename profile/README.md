# Powers Interactive

Powers Interactive is a digital advertising firm that has built its own internal operating system to run high-scale, high-compliance campaigns.

Our platform exists to create **operational leverage**, **speed**, and **auditability** in environments where complexity, regulation, and data fragmentation are the norm.

This repository space contains the core systems that power our internal workflows, data foundation, and emerging intelligence layers.

---

## Platform Overview

We structure our technology as a set of clearly separated, composable systems — each with a single responsibility.

### **/foundry**
**The Operating System**

Foundry is our internal operating system — where work happens.

It owns:
- workflow orchestration (requests, plans, launch kits)
- approvals and lifecycle enforcement
- assignments, queues, and revisions
- audit logging and override controls
- human-facing execution and decision-making

If someone at Powers takes an action, it happens in **/foundry**.

---

### **/bedrock**
**The Data Foundation**

Bedrock is the canonical data foundation beneath every other system.

It is responsible for:
- ingesting data from internal and external sources
- normalizing and reconciling entities
- enforcing tenancy and access control
- producing analytics-ready datasets

Everything downstream — reporting, intelligence, and automation — is grounded in **/bedrock**.

---

### **/atlas** *(coming later)*
**Advertising Activity Intelligence**

Atlas is the market intelligence layer built on Bedrock.

It aggregates advertising activity across platforms and data sources to answer:
- what is happening in the market
- where spend is moving
- how competitive dynamics are changing

Atlas is focused on **activity and observation**, not operations.

---

### **/cortex** *(coming later)*
**The Neural Network of the Political Economy**

Cortex is the semantic and relational intelligence layer.

It connects candidates, committees, consultants, vendors, donors, platforms, and states in a unified political data graph — enabling relationship-aware queries and LLM-driven analysis.

Atlas shows activity.
Cortex explains relationships and meaning.

---

## Design Principles

Our systems are built with a few non-negotiables:

- **Separation of concerns** — no system does two jobs
- **Workflow-first architecture** — state and transitions are explicit
- **Auditability by default** — every meaningful action is traceable
- **Composable systems** — each layer compounds the value of the one below it
- **Built for scale, not demos**

---

## Repository Structure

- `foundry/` — internal operating system and workflows
- `bedrock/` — data ingestion, modeling, and analytics foundation

Atlas and Cortex will be added as their own systems as they come online.

---

## Notes

This is an internal platform, developed to support real production workflows.
Documentation and structure prioritize clarity, correctness, and long-term maintainability over surface polish.
