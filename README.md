# CoSyn Governance

Constitutional governance specification for stacked-persona and multi-agent AI systems.

## Repository Role

`cosyn-governance` is the **public specification layer** in the CoSyn three-layer model.

This repository is for:
- governance constitution/specification
- whitepapers and governance rationale
- vendor-agnostic governance philosophy
- academic/architectural reference

This repository is **not**:
- an SDK
- a runtime implementation
- an orchestration engine
- an enterprise deployment system

Implementers are responsible for applying this specification in their own systems.

## Strategic Boundary (Authoritative)

See: `docs/REPO-BOUNDARY.md`

Public:
- `cosyn-governance` (constitution/spec)
- `cosyn-openclaw` (hardened baseline implementation)

Private:
- `cosyn-core` (strategic enforcement/orchestration/enterprise layer)

## Current Specification Artifacts

### Constitutional core
- `CoSyn_Governance_Constitution_v8.4.1_Full.md`

Normative governance source for principles, protocol stack, behavioral guarantees, and lifecycle constraints.

### Modular packaging (beta)
- `v9-modular/GOVERNANCE.md`

Structured modular packaging for stacked-persona adoption and implementation mapping.

## Usage Guidance

- Governance research/audit/policy citation → use `CoSyn_Governance_Constitution_v8.4.1_Full.md`
- Implementation mapping and integration planning → use `v9-modular/GOVERNANCE.md`

Use both when translating constitutional guarantees into system-level implementation behavior.

## Contribution Policy

- Pull requests are not accepted by default.
- Issues may be opened for clarification, interpretation, and discussion.
- Canonical governance updates are released by maintainers via explicit versioned revisions.

## Changelog for Boundary Update

See: `BOUNDARY_CHANGELOG.md`

## License

MIT. See `LICENSE`.
