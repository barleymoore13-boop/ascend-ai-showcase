# Security and Responsible AI

## Security posture

- Secrets and credentials remain outside version control and are never included in portfolio artefacts.
- Real runtime data is separated from disposable validation state.
- External integrations are bounded and failures remain visible to the user.
- Untrusted tool material is inspected without execution and unsafe conditions fail closed.
- Dependency and automation changes are reviewed as supply-chain changes, not routine version bumps.
- Publication candidates receive secret, metadata, provenance, history-isolation, and reconstruction-risk review.

## Privacy posture

The private product may handle personal career information. This showcase contains no CV, profile, application, vacancy record, database, export, log, trace, upload, cache, private URL, or absolute user path. Synthetic descriptions are used in place of real user journeys.

## Responsible AI posture

- AI output supports review; it does not replace the user's decision.
- Application submission and employer contact require deliberate human action.
- Uncertain or unavailable system states are shown honestly.
- AI-assisted engineering is recorded as provenance evidence but is not treated as automatic proof of authorship, ownership, or correctness.
- High-impact changes require tests and review appropriate to their risk.

## Disclosure boundary

This document intentionally omits exploit instructions, endpoint maps, exact defensive thresholds, prompts, provider request construction, proprietary ranking or classification logic, and raw schema details. Security concerns about a future public artefact should be reported privately to the repository owner rather than demonstrated against a live system.
