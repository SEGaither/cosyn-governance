# Repo Boundary Changelog

Date: 2026-02-26

## Summary
This repository now formally adopts the CoSyn three-layer boundary model.

### Role of `cosyn-governance` (Public, MIT)
`cosyn-governance` is the **constitutional/specification** layer.
It exists for:
- governance specs
- whitepapers
- vendor-agnostic design principles
- academic/architectural framing

It is intentionally **not** an implementation runtime or enforcement engine.

## What changed
- Added `docs/REPO-BOUNDARY.md` to codify public/private scope boundaries.

## Boundary contract
Public:
- Constitution/specification (`cosyn-governance`)
- Baseline implementation (`cosyn-openclaw`)

Private:
- Strategic enforcement/orchestration/enterprise layer (`cosyn-core`)

## Notes
This update is governance-positioning and scope-control only; no security guarantees are implied beyond explicitly documented and verified behavior in implementation repos.
