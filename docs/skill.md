# Using the ARGUS Skill

- **Stable wrapper:** 0.6.0
- **Target protocol:** ARGUS V5.1.0

The ARGUS Skill is an execution layer around the published protocol. It does not replace the protocol. If an instruction in the wrapper conflicts with the normative protocol, the protocol prevails.

## Installation

Download `skill/V0.6.0/argus-wrapper-v0.6.0.zip` or the corresponding GitHub release asset, then import the ZIP through the platform's Skill or equivalent management interface.

Platform terminology and menu locations can change. The ARGUS website maintains the current end-user installation notes.

## Usage

Full analysis:

> Analyze this text with ARGUS.

Short mode:

> Analyze this text with ARGUS Light.

Related texts:

> Analyze these texts as a corpus with ARGUS.

For an execution independent of previous analyses, use a fresh conversation and do not provide the earlier analysis.

## Package contents

The 0.6.0 archive contains:

- `argus/SKILL.md`
- `argus/wrapper-versions.md`
- `argus/agents/openai.yaml`
- `argus/references/argus-protocol-fr.md`
- `argus/references/versions-fr.md`
- `argus/references/execution-rules.md`
- `argus/references/output-template-fr.md`

## Revision 0.6.0

Revision 0.6.0 targets ARGUS V5.1.0. It formalizes analyst provenance through model, version/build and reasoning intensity, retains host and execution-regime metadata, and records reasoning intensity using the provider's own label without cross-provider normalization.

The analytical rules of the modal-constancy detector belong to the V5.1.0 protocol, not to the wrapper. The wrapper adds the corresponding execution/restitution requirements, including confidence signalling near the acknowledged-revision / disguised-retraction boundary.

The final ZIP uses portable `/` entry separators and was successfully accepted by Claude.

## Tested and validated hosts

Revision 0.4.2 received the documented cross-host smoke test with ChatGPT 5.6 and Claude Opus 5.

Revision 0.5.0 was validated as a non-regressive wrapper migration targeting V5.0.0.

Revision 0.6.0 was structurally validated for V5.1.0, and its final portable ZIP was successfully imported by Claude.

Execution quality still depends on the host environment: effective context, output capacity, document ingestion, access to external sources, and persistence of instructions over a long execution.
