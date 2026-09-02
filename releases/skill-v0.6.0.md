# ARGUS Skill 0.6.0

- **Release date:** 2026-09-02
- **Target protocol:** ARGUS V5.1.0
- **Status:** stable

ARGUS Skill 0.6.0 is the stable execution wrapper for ARGUS Protocol V5.1.0.

The Skill does not replace the protocol. The analytical rules of the modal-constancy detector belong to ARGUS V5.1.0; wrapper 0.6.0 updates the execution layer and analyst-provenance metadata.

## Changes in 0.6.0

- Updates the target protocol from ARGUS V5.0.0 to **ARGUS V5.1.0**.
- Formalizes analyst provenance in three fields: **model**, **version/build**, and **reasoning intensity**.
- Retains existing execution metadata, including **host** and **execution regime**.
- Records reasoning intensity using the provider's own label, verbatim and without cross-provider normalization; uses **not exposed** when the environment exposes no such value.
- Requires confidence to be signalled when a modal-constancy verdict lies near the boundary between **acknowledged revision** and **disguised retraction**.

## Validation and portability

The final 0.6.0 archive was structurally validated and successfully imported by Claude after enforcing portable POSIX-style ZIP entry paths (`/` rather than Windows `\`). The packaged French protocol is byte-identical to the normative V5.1.0 French source published with this release.

## Download integrity

`argus-wrapper-v0.6.0.zip`

File size: **83,231 bytes**

SHA-256:

`949a375fc3a52b1c402e4026e843cb58a2a5d935253cf4fb3da6324f170ce817`
