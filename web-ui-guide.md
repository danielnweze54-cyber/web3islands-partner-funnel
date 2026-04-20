# NeuroChain DSL Web UI Guide

## Overview

The NeuroChain DSL Web UI provides a visual interface for interacting with deterministic workflows...

Unlike traditional AI systems that rely on free-form outputs, NeuroChain enforces a transparent, step-based execution model where everyactionisdefined, validated, observable.

---

## Core Concepts

NeuroChain is built around four key principles:

- **Deterministic Execution** — every request follows a predictable flow
- **Action Plans (DSL)** — user input is converted into structured steps
- **Guardrails** — safety checks applied at each step
- **Local Classification** — decisions are validated before execution

This ensures that users are not interacting with a “black box,” but with a controlled and inspectable system.

---

## Web UI Experience

The Web UI is designed to make the execution process **visible and understandable**.

Instead of showing only input/output, it exposes:

- The generated **Action Plan**
- The **state of each step**
- The **validation process (guardrails)**
- The **final execution result**

This allows users to follow exactly what the system is doing.

---

## User Flow

### 1. Input

The user submits a request through the interface.

This acts as the trigger for generating a structured execution flow.

---

### 2. Action Plan Generation

The system converts the request into a **DSL-based Action Plan**.

Each step is explicitly defined and visible in the UI.

Example structure:
- Parse input
- Validate intent
- Prepare execution
- Execute action

The key idea is that the plan is:
- deterministic
- inspectable
- structured

---

### 3. Guardrail States

Before execution, each step is evaluated through guardrails.

In the UI, this can be represented through states such as:

- **Pending** — step not yet evaluated  
- **Validated** — step approved for execution  
- **Rejected** — step blocked by safety rules  

This stage is critical, as it prevents unsafe or undefined behavior.

---

### 4. Execution Flow

Once validated, the Action Plan is executed step by step.

The UI reflects:
- progression through steps
- current active step
- completed steps

This makes execution **traceable and transparent**.

---

### 5. Result & Traceability

After execution, the result is returned along with the full trace.

Users can:
- review the Action Plan
- see which steps passed or failed
- understand how the output was produced

---

## Safety Model

NeuroChain enforces safety through layered control:

### Deterministic DSL
All actions must conform to predefined logic.

### Guardrails
Each step is validated before execution.

### Local Classification
Decisions are checked locally to avoid unsafe outcomes.

---

## Why This Approach Matters

Traditional AI systems:
- produce unpredictable outputs  
- hide internal reasoning  

NeuroChain:
- enforces structured execution  
- exposes internal steps  
- ensures safety before action  

This shifts AI interaction from **guesswork → controlled systems**.

---

## UI Representation

In the Web UI, the system is visualized through interactive components:

- **ActionPlan Panel**  
  Displays the full execution plan as a step-by-step list.

- **Step States**  
  Each step updates in real time:
  - Pending → Running → Completed / Rejected

- **Guardrail Indicators**  
  Validation status is shown alongside each step to indicate approval or failure.

- **Execution Status**  
  A final state (Success / Failed) provides immediate feedback to the user.

This visual structure ensures that users not only understand the system logically, but can also follow execution in real time through the interface.

## Summary

The NeuroChain DSL Web UI transforms AI interaction into a **transparent, step-based workflow**.

Users can:
- see how decisions are made  
- verify execution steps  
- trust the system through visibility and control  

It is not just an interface — it is a tool for **understanding and validating execution in real time**.
