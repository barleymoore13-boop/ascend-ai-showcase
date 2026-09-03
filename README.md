# Ascend AI — Quiet Growth Showcase

Ascend AI is a private, Mac-first career decision-support project. This repository is a deliberately limited public showcase of the Quiet Growth landing page and approved synthetic-data demonstration video; it does not publish product source code, private data, provider integrations, security internals, or Git history.

## Product intent

Ascend helps a person organise job-search information, assess opportunities, and prepare application material while keeping consequential actions under human control. It is designed to make uncertain system states visible rather than presenting unavailable or disabled services as successful results.

## What this showcase demonstrates

- evidence-first debugging and narrowly scoped fixes;
- local runtime and test-data isolation on macOS;
- truthful UI states for disabled, failed, empty, and successful operations;
- defensive treatment of untrusted tools and dependency risk;
- human approval before application submission or employer contact;
- IP, asset-provenance, and publication-safety review;
- documented regression evidence and release decision gates.

## Verified engineering evidence

The following results were recorded on 20 August 2026 against the private project and are presented as dated evidence, not as a public test harness:

- a focused external-tool security gate: **6 passed**;
- a fresh isolated Python dependency audit: **no known vulnerabilities found**;
- a macOS runtime/truthfulness regression: **44 focused tests passed**;
- the corresponding private full Python suite: **439 passed, 28 skipped**;
- a disposable Chromium regression: **12 passed**.

The private product, its tests, dependencies, schemas, and CI workflows are intentionally not copied here.

## Safe public documentation

- [Case study](docs/CASE_STUDY.md)
- [Architecture overview](docs/ARCHITECTURE_OVERVIEW.md)
- [Engineering highlights](docs/ENGINEERING_HIGHLIGHTS.md)
- [Security and responsible AI](docs/SECURITY_AND_RESPONSIBLE_AI.md)
- [Publication allowlist](PUBLICATION_ALLOWLIST.md)
- [Deliberate omissions](OMISSIONS.md)

## Publication status

This showcase is publicly available for portfolio and engineering-review purposes. The underlying Ascend AI product remains private, and no open-source licence is asserted or implied.
