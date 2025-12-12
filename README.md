# CoSyn Governance Stack

Constitutional governance for stacked-persona and multi-agent AI systems.

CoSyn is a **behavioral governance layer**, not another agent framework or SDK.
It defines how AI personas behave, how they are routed, and how drift is detected and constrained.

CoSyn is written as a **vendor-agnostic governance spec**: the same constitution can be adopted across independent stacks or organizations, providing a shared rulebook for multi-agent systems without depending on a single platform, including decentralized or other multi-party environments.

As systems grow, the same constitution can be applied across many personas, teams, and deployments, giving organizations a **repeatable governance substrate** and a consistent way to surface drift, risk, and audit trails, suitable for regulated or other high-stakes contexts.

---

## One sentence

CoSyn is a **governance constitution + stacked-governance packaging** that lets you run growing numbers of AI personas in one system with clear boundaries, auditability, and repeatable behavior—across tools, teams, and deployments.

---

## Current status — December 2025

* **CoSyn Governance Constitution v8.4.1**
  Canonical governance text for the CoSyn 8.x line.
  The 8.x governance stack has been iterated and enforced internally across many projects for ~18 months; v8.4.1 is the current consolidated version of that lineage.

* **v9 Modular (Stacked Governance)**
  A modular packaging of that same 8.4.1 constitution for:

  * stacked-persona projects
  * project-file persona sets
  * GPT / LLM systems that load persona instruction files.
    v9 is published as a **public beta specification**, open to community testing and feedback.

All contents in this repository are released under the **MIT license**.

---

## What this repo contains

### 1. Constitutional core (v8.4.1)

* `CoSyn_Governance_Constitution_v8.4.1_Full.md`

This file is the **full CoSyn governance constitution**:

* principles
* protocol stack (SCP, SFP, BTP, PRAP, PSD-1, DDP, UDN, RLP, etc.)
* behavioral guarantees
* lifecycle rules for personas

If you want to **understand CoSyn**, start here.
If you are building your own implementation, this is the **normative source of truth**.

Because it is tool- and vendor-agnostic, the v8.4.1 constitution can be used as a **shared governance specification** across multiple systems, organizations, or agent frameworks.

---

### 2. Stacked governance packaging (v9 Modular)

* `v9-modular/GOVERNANCE.md`

This file takes the **same v8.4.1 constitution** and:

* reorganizes it into **modules** (core protocols, addenda, application rules, implementation notes)
* adds the **Persona Invocation Protocol (PIP)** for persona files stored in project artifacts
* defines how CoSyn applies to:

  * chat-based personas
  * project-file persona sets
  * stacked-persona agent / GPT systems

Think of it as:

* v8.4.1 = **what** the system must do
* v9 Modular = **how** to apply it cleanly in stacked-persona architectures

The v9 spec is labeled **beta** so changes can be made in response to real-world use without implying a change to the underlying constitution.

---

## When to use which file

* **You are doing governance research, audits, or policy work**
  → Read **`CoSyn_Governance_Constitution_v8.4.1_Full.md`**
  (the constitution is the artifact that should be cited in papers and governance docs, and can serve as a common reference across tools or organizations).

* **You are a developer wiring CoSyn into a project or framework**
  → Start with **`v9-modular/GOVERNANCE.md`**
  and map its modules into:

  * your persona definitions
  * your routing and orchestration layer
  * your logging / audit layer.

This repository provides **specifications**, not an SDK or runtime library.
Implementers are responsible for applying the governance rules within their own codebases and frameworks.

* **You need to prove what v8.4.1 means in a concrete system**
  → Use both:

  * the constitution file (behavioral guarantees), and
  * the modular file (concrete application to stacked-persona systems).

---

## Typical use cases

CoSyn is **framework-agnostic**. It is designed to be implemented **under** existing tools, including (for example):

* LangChain or LlamaIndex–based pipelines
* custom multi-agent / orchestrator code
* GPTs or local LLMs with many specialized personas
* internal AI “C-Suite” or expert teams

You keep your current tools.

CoSyn provides:

* a **constitution** for how agents/personas should behave (v8.4.1), and
* a **stacked governance specification** for how they should be routed and audited (v9-modular).

Because the same constitution can be applied across many personas and deployments, organizations can:

* run multiple AI roles or agents with **consistent governance**,
* detect and surface drift using a shared protocol stack,
* and align internal teams, vendors, or business units on **one written rulebook** instead of ad-hoc, tool-specific behavior.

---

## Roadmap (high-level)

The open-source parts in this repo are intended to stay:

* **free** (MIT)
* **small** and easy to read
* focused on **governance, not infrastructure**

Planned additions (all optional, separate from this repo):

* example persona files + registry format
* minimal routing patterns for stacked personas (spec or pseudo-code)
* conceptual integration notes for common Python agent frameworks

Closed/commercial work (not in this repo):

* enterprise audit dashboards and drift logs
* EU AI Act / SOC-2 oriented compliance bundles
* one-click cloud deployers
* custom persona stacks and support contracts

---

## License

This repository is licensed under the **MIT License**.
See `LICENSE` for full details.
