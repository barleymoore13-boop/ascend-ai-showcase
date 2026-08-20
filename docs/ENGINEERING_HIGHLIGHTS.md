# Engineering Highlights

## Truthful product states

A disabled search path once appeared equivalent to a completed scan with zero results. The correction introduced an explicit disabled outcome across the service and interface boundary. Freshness was also recalculated when results were presented so time-dependent status could not remain indefinitely stale.

## macOS runtime work

The local launcher was reviewed as part of the complete runtime path rather than as an isolated script. Live and offline modes became explicit, invalid modes fail early, and responsive behaviour was covered in a disposable browser environment. An already-running real process was not interrupted during validation.

## Test and runtime isolation

Browser validation uses a disposable runtime and a dedicated loopback test endpoint. The normal local service and real user state remain outside that boundary. Protected-state snapshots and cleanup checks form part of the validation evidence.

## Security and supply chain

The dependency incident was handled by distinguishing direct from transitive packages, resolving compatible patched versions in isolation, and auditing the resolved environment. The CI workflow uses least-privilege read access and supported action runtimes. An external-tool gate inspects risky trees without executing them and fails closed on unsafe filesystem conditions.

## Data provenance design

Before changing a live schema, the existing database lifecycle was traced and tested with disposable state. The resulting plan begins with a read-only manifest: canonical schema hash, row counts, format version, and optional consistent snapshot hash, with no raw private rows or absolute paths. Migration ledgers remain a later phase behind backup-and-restore proof.

## IP and release engineering

The project maintains a clear separation between engineering evidence and legal conclusions. Unresolved assets are excluded, third-party licence evidence is treated as release-specific, AI contribution metadata is not presented as proof of ownership, and public publication remains a human approval boundary.

## Dated validation snapshot

On 20 August 2026, the private project recorded:

- 6 passing focused external-tool security tests;
- a clean isolated dependency audit;
- 44 passing focused macOS/runtime tests;
- 439 passing and 28 skipped tests in the corresponding full Python suite;
- 12 passing disposable Chromium tests.

These figures are scoped historical evidence. This showcase contains no copied test suite and makes no claim that public readers can reproduce the private product from it.
