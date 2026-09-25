# ENTITY-AI

**ENTITY v3.4.0 executable AI implementation package.**

This repository configures the **one ENTITY Global Passport** for AI systems, models, datasets, derived outputs and related governance artifacts. It does not define a separate passport protocol and does not modify ENTITY core semantics.

[ENTITY](https://github.com/blackmore-technology-group/ENTITY) · [v3.4.0 release](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.0) · [Global Passport documentation](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/v3.4/GLOBAL_PASSPORT.md) · [Domain packages](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/v3.4/DOMAIN_PACKAGES.md)

## What this package is for

Use ENTITY-AI as the starting point when you need persistent provenance, scoped authority, rights and evidence around AI-related assets while keeping model custody, hosting and platform control separate from sovereign authority.

The v3.4 package includes mappings for **NIST AI RMF**, **SPDX 3** and **CycloneDX**. Those mappings describe correspondence; ENTITY does not redefine the external standards or turn a mapping into certification or regulatory compliance by itself.

Typical evaluation paths include:

- carrying origin, authority and evidence context with models, datasets or derived outputs;
- recording rights and usage constraints across training, inference or downstream derivation;
- preserving provenance through provider or platform changes;
- composing jurisdiction, privacy, trust, technical and AI-domain profiles inside one Global Passport.

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

The verifier checks the repository inventory and the package/source-release binding.

## Release binding

- Core source: `blackmore-technology-group/ENTITY` PR #41
- Source head: `2d7529fbadb4dd04840d62b751294bf9a7f70ed5`
- Release snapshot: `3ff0e51ca2daabf50bc517e9c6e3438e8c150f1560cca6c99621621e3c855a90`
- Package SHA-256: `4877cb5bc76ef0803eace931ca1a9cba516c01ba94a2e0b4bc71bcb5dc1b0440`

## Go deeper

- [ENTITY v3.4.0](https://github.com/blackmore-technology-group/ENTITY/releases/tag/v3.4.0)
- [Developer portal](https://github.com/blackmore-technology-group/ENTITY/blob/main/DEVELOPERS.md)
- [Engineering evidence](https://github.com/blackmore-technology-group/ENTITY/blob/main/docs/ENGINEERING_EVIDENCE.md)
- [Open contributor tasks](https://github.com/blackmore-technology-group/ENTITY/issues?q=is%3Aissue+is%3Aopen)

## Truth and compliance boundary

External standards remain externally authoritative and are mapped, not redefined. Package verification does **not** establish regulatory compliance, objective external truth, model safety, legal title or accounting fair value. Provider custody or model hosting does not create ENTITY authority.

Deployment-specific legal, regulatory, safety, security and model-governance determinations remain the responsibility of the deploying organization.
