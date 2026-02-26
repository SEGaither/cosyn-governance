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

## Governance Version Positioning

- **Current canonical runtime governance source:** CGS v10.2.0 JSON bundle (local governance binding)
- **Public modular textual specification:** CGS v9.0 (`v9-modular/GOVERNANCE.md`)
- **Lineage continuity:** v8.4 → v8.4.1 → v9.0 → v10.2.0

Use `VERSION_MANIFEST.md` as the authoritative version/lineage reference for this repo.

## Current Specification Artifacts

### Constitutional core
- `CoSyn_Governance_Constitution_v8.4.1_Full.md`

### Modular packaging (public text)
- `v9-modular/GOVERNANCE.md`

## Usage Guidance

- Governance research/audit/policy citation → use constitutional and modular spec artifacts in this repo.
- Runtime binding/version authority for current stack → use canonical JSON governance bundle declarations in version docs.

## Contribution Policy

- Pull requests are not accepted by default.
- Issues may be opened for clarification, interpretation, and discussion.
- Canonical governance updates are released by maintainers via explicit versioned revisions.

## Changelog for Boundary Update

See: `BOUNDARY_CHANGELOG.md`

## Version Manifest

See `VERSION_MANIFEST.md` for canonical version lineage and compliance labeling.

## License

MIT. See `LICENSE`.
