# STRUCTURE — cosyn-core (Private Strategic Layer)

`cosyn-core` is the private strategic repository for CoSyn.

## Purpose

This repo contains proprietary implementation layers that are intentionally excluded from public baseline repositories.

## What belongs here

- Enforcement engine internals
- Multi-agent orchestration runtime
- Drift/risk scoring models
- Enterprise adapters and deployers
- Compliance bundles and policy packs
- Runtime automation and operational controls

## What does NOT belong here

- Public constitutional/spec-only content (belongs in `cosyn-governance`)
- Public baseline profile/reference onboarding content (belongs in `cosyn-openclaw`)

## Collaboration posture

- Private by default
- Access by maintainer approval
- Contribution and commercialization terms defined per agreement

## Release boundary (authoritative)

- `cosyn-governance` (PUBLIC): ideas/specification/philosophy
- `cosyn-openclaw` (PUBLIC): hardened baseline only
- `cosyn-core` (PRIVATE): strategic enforcement/orchestration/enterprise layer

If uncertainty exists about placement, default to private and request boundary review.
