# ENTITY-AI

**Sealed ENTITY v3.4.0 AI implementation package, evaluated in the current ENTITY v3.4.2 ecosystem.**

**Current canonical core release:** [ENTITY v3.4.2 — Canonical BTDU Release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.2).

The sealed domain-package payload in this repository remains the historical v3.4.0 package. Its recorded package-specific requalification against v3.4.1 remains historical evidence; this README does not silently rewrite that evidence into a new v3.4.2 package qualification. The current v3.4.2 adoption path is documented and open for clean-clone external evaluation.

This repository configures the **one ENTITY Global Passport** for AI systems, models, datasets, derived outputs and related governance artifacts. It does not define a separate passport protocol and does not modify ENTITY core semantics.

[ENTITY](https://github.com/blackmore-technology-group/ENTITY) · [v3.4.2 release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.2) · [ENTITY documentation](https://blackmore-technology-group.github.io/ENTITY-DOCS/) · [AI domain documentation](https://blackmore-technology-group.github.io/ENTITY-DOCS/domains/ai.html) · [AI agent authorization guide](https://blackmore-technology-group.github.io/ENTITY-DOCS/guides/ai-agent-authorization-governance.html) · [Domain-package evaluation task](https://github.com/blackmore-technology-group/ENTITY/issues/46)

## What this package is for

Use ENTITY-AI as the starting point when you need persistent provenance, scoped authority, rights and evidence around AI-related assets while keeping model custody, hosting and platform control separate from sovereign authority.

The sealed package includes mappings for **NIST AI RMF**, **SPDX 3** and **CycloneDX**. Those mappings describe correspondence; ENTITY does not redefine the external standards or turn a mapping into certification or regulatory compliance by itself.

Typical evaluation paths include:

- carrying origin, authority and evidence context with models, datasets or derived outputs;
- recording rights and usage constraints across training, inference or downstream derivation;
- preserving provenance through provider or platform changes;
- composing jurisdiction, privacy, trust, technical and AI-domain profiles inside one Global Passport;
- testing whether an authenticated AI agent can act outside explicitly delegated authority.

## Deploy the package

Required deployment facts:

- `organization`
- `jurisdiction`
- `authority_source`
- `model_governance_policy`

`deployment.example.json` is intentionally non-production until every `CONFIGURE-ME` value is replaced with organization-specific facts.

```text
Select package → configure organization facts → connect systems/data → ingest → verify passport → run conformance → deploy
```

## Verify locally

```bash
python tools/verify_package.py
```

The verifier checks the repository inventory and the sealed package/source-release binding. A successful package verification does not, by itself, establish a new v3.4.2 qualification claim.

## Sealed package provenance

- Core source: `blackmore-technology-group/ENTITY` PR #41
- Source head: `2d7529fbadb4dd04840d62b751294bf9a7f70ed5`
- Release snapshot: `3ff0e51ca2daabf50bc517e9c6e3438e8c150f1560cca6c99621621e3c855a90`
- Package SHA-256: `4877cb5bc76ef0803eace931ca1a9cba516c01ba94a2e0b4bc71bcb5dc1b0440`

These values describe the sealed historical package payload and should not be rewritten merely because the current core release advances.

## Current evaluation path

- [ENTITY v3.4.2 core release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.2)
- [ENTITY v3.4.2 + BTDU documentation](https://blackmore-technology-group.github.io/ENTITY-DOCS/v342/)
- [AI domain manual](https://blackmore-technology-group.github.io/ENTITY-DOCS/domains/ai.html)
- [AI governance and provenance guide](https://blackmore-technology-group.github.io/ENTITY-DOCS/guides/ai-governance-provenance.html)
- [AI-agent authorization guide](https://blackmore-technology-group.github.io/ENTITY-DOCS/guides/ai-agent-authorization-governance.html)
- [Try one current domain-package path from a clean clone](https://github.com/blackmore-technology-group/ENTITY/issues/46)
- [External verification challenge](https://github.com/blackmore-technology-group/ENTITY/issues/55)

## Truth and compliance boundary

External standards remain externally authoritative and are mapped, not redefined. Package verification does **not** establish regulatory compliance, objective external truth, model safety, legal title or accounting fair value. Provider custody or model hosting does not create ENTITY authority.

Deployment-specific legal, regulatory, safety, security and model-governance determinations remain the responsibility of the deploying organization.
