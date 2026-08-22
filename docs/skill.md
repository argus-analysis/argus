# Using the ARGUS Skill

**Stable wrapper:** 0.4.3  
**Target protocol:** ARGUS V5.0.0

The ARGUS Skill is an execution layer around the published protocol. It does not replace the protocol. If an instruction in the wrapper conflicts with the normative protocol, the protocol prevails.

## Installation

Download `skill/V0.4.3/argus-0.4.3.zip` or the corresponding GitHub release asset, then import the ZIP through the platform's Skill or equivalent management interface.

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

The 0.4.3 archive contains:

- `argus/SKILL.md`
- `argus/agents/openai.yaml`
- `argus/references/argus-protocol-fr.md`
- `argus/references/versions-fr.md`
- `argus/references/execution-rules.md`
- `argus/references/output-template-fr.md`

## Tested hosts

Revision 0.4.2 was tested on August 21, 2026 with ChatGPT 5.6 and Claude Opus 5 on a full ARGUS analysis of the same article. Both executions applied the wrapper's substantive corrections and reached the same ARGUS 7.c level.

Revision 0.4.3 is a technical portability update for source and analyzed-object links. The packaged Skill was structurally validated before publication; no new protocol rule or analytical category was introduced.

Execution quality still depends on the host environment: effective context, output capacity, document ingestion, access to external sources, and persistence of instructions over a long execution.
