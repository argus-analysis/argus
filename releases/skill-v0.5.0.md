# ARGUS Skill 0.5.0

**Release date:** 2026-08-26  
**Target protocol:** ARGUS V5.0.0  
**Status:** stable

ARGUS Skill 0.5.0 is the stable execution wrapper for ARGUS Protocol V5.0.0.

The Skill does not replace the protocol. ARGUS V5.0.0 remains the normative reference and is unchanged in this release.

## Changes in 0.5.0

- Clarifies neutral input: an ARGUS analysis does not require a user-supplied analytical question, hypothesis or prior orientation.
- Adds execution metadata for model, host and execution regime.
- Distinguishes wrapper execution from context-only execution.
- Adds the publication-layer rules used by ARGUS Case Studies without creating a new analytical mode.
- Adds a dedicated wrapper version history.
- Preserves all analytical rules, verification requirements, corpus rules and conclusion categories of ARGUS V5.0.0.

## Validation

Version 0.5.0 was produced as a controlled migration from wrapper 0.4.3.

The migration passed the complete non-regression control set:

- protected normative files unchanged;
- no operational 0.4.3 version residue;
- all expected version declarations updated;
- nine non-regression witnesses preserved;
- no line removed except the five explicit wrapper-version replacements.

The final candidate was independently audited after these mechanical controls.

## Download integrity

`argus-0.5.0.zip`

File size: 76,177 bytes

SHA-256:

`e5c212bacc4b052ba62f0d45ec0cf5b9b4973a39de63ef4203f258f805865344`
