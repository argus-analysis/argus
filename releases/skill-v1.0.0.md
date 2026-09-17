# ARGUS Skill 1.0.0

- **Release date:** 2026-09-17
- **Target protocol:** ARGUS V5.1.0
- **Status:** stable

ARGUS Skill 1.0.0 is the first stabilized public boundary of the generic execution wrapper for ARGUS Protocol V5.1.0.

The Skill does not replace the protocol. ARGUS V5.1.0 remains the normative analytical reference; wrapper 1.0.0 changes execution safeguards and public wrapper scope only.

## Changes in 1.0.0

- Establishes a site-independent public wrapper boundary: the generic wrapper contains ARGUS execution guidance only.
- Removes site-specific Case Study, publication-synthesis and editorial-pipeline conventions from the public wrapper; those belong in separate tooling.
- Retains the generic 0.6.0 execution layer, including analyst provenance, host and execution-regime metadata, source-reference portability, segmentation guidance and environment-capability checks.
- Requires every Step 8 correction that affects a mechanism used in Step 7.c to propagate into the terminal judgment.
- At the Level 2 / Level 3 boundary, requires an explicit demonstration of effective convergence rather than a count or accumulation of defects, with a symmetric demonstration when Level 2 is retained.
- Adds inter-pass state integrity: a finding explicitly frozen in an earlier adjudication pass remains an operative premise unless a demonstrable factual contradiction or a material element previously unavailable is identified and cited.
- Keeps the normative target unchanged at **ARGUS V5.1.0**.

## Development history

The 0.7.0 line was a development branch used to experiment with publication-specific orchestration. It was never released as the stable successor to 0.6.0. Its publication-specific work was separated from the public wrapper before 1.0.0.

## Validation and portability

The 1.0.0 package was produced by controlled migration from the complete wrapper lineage and validated as the final RC3 candidate before promotion. Structural validation, ZIP integrity, exact package/tree comparison, reverse migration to the prior release candidate and acceptance/non-regression checks all passed. The bundled French protocol is byte-identical to the normative ARGUS V5.1.0 French source.

The archive uses portable POSIX-style ZIP entry paths (`/`).

## Download integrity

`argus-wrapper-v1.0.0.zip`

File size: **86,210 bytes**

SHA-256:

`8e48404edfc95371191825ca77a06c5ce7b62dba71aa85aff415dd2e6a321cef`
