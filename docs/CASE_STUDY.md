# Case Study

## The problem

Job searching combines incomplete information, repetitive research, document preparation, and high-consequence decisions. A useful assistant must reduce that friction without inventing certainty or taking control away from the applicant.

## Product principles

Ascend was engineered around five principles:

1. **Truth before polish.** Disabled, failed, empty, and successful operations must remain distinguishable.
2. **Human control.** The person reviews and submits applications; automation does not contact employers.
3. **Local privacy.** Mutable user state is kept in a protected local runtime and test runs use disposable storage.
4. **Evidence before change.** Reproduce a defect, make the smallest correction, and validate in proportion to risk.
5. **Publication restraint.** Portfolio evidence should demonstrate judgement without exposing protected implementation or user data.

## User journey

A typical synthetic journey is:

1. review or collect opportunity information;
2. inspect freshness and source confidence;
3. compare an opportunity with the user's goals;
4. prepare supporting material for human review;
5. let the user decide whether and where to apply.

No live vacancy, employer identity, CV, application, or personal profile is included in this showcase.

## Engineering approach

The project evolved through repeated evidence loops: diagnose the observed failure, separate provider failure from a genuine empty result, preserve runtime isolation, add focused regression coverage, and then run broader suites only when the change risk justified them.

The same approach was used for supply-chain work. Dependency relationships were inspected before upgrades, audit fixes were verified in a clean environment, and CI actions were moved to supported runtimes without bundling the private workflow here.

## What changed in practice

Examples of engineering outcomes include:

- a Mac launcher that distinguishes live and explicit offline operation;
- UI states that do not disguise disabled search as a successful zero-result scan;
- time-sensitive vacancy freshness recalculated when results are presented;
- responsive layout coverage at common Mac viewport sizes;
- fail-closed inspection of untrusted external tool trees;
- read-first database provenance design before any migration was considered.

## Lessons

- A green-looking UI can still be misleading if backend outcome states are collapsed.
- Local-first software needs explicit boundaries between real runtime data and disposable validation.
- A public portfolio can show rigorous engineering more safely through decisions and evidence than through wholesale source release.
- IP and provenance work belongs inside release engineering, not at the end as an afterthought.
