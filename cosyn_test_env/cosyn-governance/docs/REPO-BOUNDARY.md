# Repo Boundary Policy (CoSyn)

This document defines the strategic repository split for CoSyn.

## Public Repositories

### 1) `cosyn-governance` (PUBLIC, MIT)
Purpose:
- Constitutional specification
- Whitepapers
- Vendor-agnostic governance philosophy
- Academic and architectural positioning

Why public:
- Establishes authorship and citability
- Builds credibility and thought leadership
- Safe to publish under MIT because this repo is specification-oriented, not an enforcement engine

Boundary:
- Do not include implementation runtimes or proprietary orchestration logic.

### 2) `cosyn-openclaw` (PUBLIC when verification is complete)
Purpose:
- Hardened baseline implementation
- Reference configuration
- Community onboarding
- Practical adoption path

Why public:
- Drives adoption
- Demonstrates practical governance execution
- Attracts contributors and users

Release condition for public baseline claims:
- Verification evidence complete
- Claims constrained to verified behavior
- No proprietary orchestration/enforcement logic

Boundary:
- Baseline only. Never evolve this repo into a full enforcement runtime or enterprise platform.

## Private Repository

### 3) `cosyn-core` (PRIVATE)
Purpose:
- Advanced enforcement engine
- Orchestration layer
- Drift scoring model
- Enterprise deployment framework
- Compliance bundles
- Runtime automation

Why private:
- Strategic leverage
- Monetizable implementation layer
- Collaboration and compensation boundary

Boundary:
- Keep private unless released under explicit structured agreement.

## Strategic Rule

Public:
- The Constitution (`cosyn-governance`)
- The Baseline (`cosyn-openclaw`)

Private:
- The Engine (`cosyn-core`)
- Enterprise/compliance layer
- Operational multiplier

## Critical Guardrail

`cosyn-openclaw` must never contain:
- Full enforcement runtime
- Adaptive governance engine
- Enterprise compliance system

If scope drift is detected, stop and move strategic content to `cosyn-core` under explicit approval.
