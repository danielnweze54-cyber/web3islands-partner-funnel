# NeuroChain DSL Web UI Guide (Core)

## Overview

The NeuroChain DSL Web UI is an interface for writing, executing, and inspecting deterministic scripts built with the NeuroChain DSL.

Unlike traditional AI interfaces that return opaque results, this UI exposes the full execution process, including:

- Script logic  
- AI-generated values  
- Execution steps  
- Logs and errors  

The goal is to provide a transparent and controlled environment for combining AI with deterministic execution.

---

## What the Web UI Is For

The Web UI allows users to:

- Write and run `.nc` scripts  
- Execute deterministic workflows step-by-step  
- Integrate AI outputs into structured logic  
- Inspect execution results, logs, and errors in real time  

It acts as a bridge between AI and deterministic systems, ensuring that AI is used as a tool — not as an uncontrolled decision-maker.

---

## Core Concepts

### 1. NeuroChain DSL Scripts (`.nc`)

Users interact with the system by writing `.nc` scripts.

These scripts define:

- Execution steps  
- Variable assignments  
- AI interactions  
- Macros and reusable logic  

Execution is deterministic, meaning:

- The structure is fixed  
- Behavior is predictable  
- Results are traceable  

---

### 2. Running a Script

Typical flow in the Web UI:

 → Clicks "Run"
 → Execution begins
 → Logs and outputs are displayed
 → AI-generated values are inserted into the flow 
→ Final result is returned

Each step is visible to the user, ensuring full transparency.

---

### 3. AI Integration

NeuroChain integrates AI in a controlled way through explicit DSL instructions.

#### `set variable from AI`

Assigns a variable using AI output.

Example:

set summary from AI

In the UI:

- AI response is displayed  
- Assigned variable is visible  
- Value can be inspected before further use  

---

#### `macro from AI`

Generates new DSL logic dynamically.

Example:

generate macro from AI

In the UI:

- Generated macro is shown  
- Resulting DSL code is displayed  
- Structure can be inspected before execution continues  

---

#### Generated Macro DSL

AI-generated macros are:

- Explicitly shown in the UI  
- Treated as part of execution  
- Never hidden  

This ensures full transparency and auditability.

---

## Execution Visibility

### Outputs
- Final script results  
- Returned values  

### Logs
- Step-by-step execution  
- Intermediate states  

### Errors
- Execution failures  
- Invalid operations  
- AI-related issues  

Everything is clearly displayed for debugging and understanding.

---

## Example UI Flow

→ Script execution starts
 → AI generates a variable
 → Variable is displayed in UI
 → Macro is generated from AI
 → Generated DSL is shown
 → Execution continues
 → Logs update in real time
 → Final output is returned

---

## Templates and Examples

The Web UI should include:

- Basic script execution  
- AI variable assignment examples  
- Macro generation examples  
- Combined workflows  

Templates should be:

- Simple  
- Readable  
- Focused on core DSL features  

---

## Safety & Control Principles

### What the UI Guarantees

- All execution is visible  
- AI outputs are explicitly shown  
- Generated logic is inspectable  
- Execution follows deterministic rules  

---

### What the UI Must NOT Do

- ❌ No hidden execution  
- ❌ No automatic actions without user trigger  
- ❌ No bypassing runtime validation  
- ❌ No silent AI decisions  

Users must always:

- See what is happening  
- Understand why  
- Control execution  

---

## Why This Matters

Traditional AI systems:

- Hide reasoning  
- Produce unpredictable outputs  

NeuroChain DSL:

- Enforces structure  
- Exposes execution  
- Controls AI usage

Black-box AI → Transparent system

---

## Extension: Stellar Layer (Context)

Once the core DSL is understood, additional layers like Stellar can be introduced.

This layer adds:

- Intent-based execution  
- Blockchain actions  
- Policy enforcement  
- Transaction handling  

But the foundation remains:

→ Deterministic DSL + Transparent AI interaction  

---

## Summary

The NeuroChain DSL Web UI enables:

- Writing deterministic scripts  
- Safe AI integration  
- Real-time execution visibility  
- Full transparency and control  

It transforms AI interaction into a structured, verifiable system.