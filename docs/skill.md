# Using the ARGUS Skill

- **Stable wrapper:** 1.0.0
- **Target protocol:** ARGUS V5.1.0

The ARGUS Skill is an execution layer around the published protocol. It does not replace the protocol. If an instruction in the wrapper conflicts with the normative protocol, the protocol prevails.

## Installation

Download `skill/V1.0.0/argus-wrapper-v1.0.0.zip` or the corresponding GitHub release asset, then import the ZIP through the platform's Skill or equivalent management interface.

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

The 1.0.0 archive contains:

- `argus/SKILL.md`
- `argus/wrapper-versions.md`
- `argus/agents/openai.yaml`
- `argus/references/argus-protocol-fr.md`
- `argus/references/versions-fr.md`
- `argus/references/execution-rules.md`
- `argus/references/output-template-fr.md`

## Version 1.0.0

Version 1.0.0 is the first stabilized public boundary of the generic ARGUS execution wrapper. It targets ARGUS V5.1.0 and deliberately excludes site-specific Case Study, publication-synthesis, translation-pipeline and editorial-workflow conventions. Those may exist in separate tooling, but they are not requirements of ARGUS execution.

The generic execution rules retained from 0.6.0 include analyst provenance, host and execution-regime metadata, source-reference portability, segmentation guidance and environment-capability checks.

The 1.0.0 hardening adds two execution safeguards without changing the normative protocol:

- a Step 8 correction that removes, lowers or reclassifies a finding used in Step 7.c must propagate into the terminal judgment; at the Level 2 / Level 3 boundary, the wrapper requires an explicit demonstration of effective convergence rather than a count of defects, with a symmetric demonstration when Level 2 is retained;
- in a multi-pass adjudication, confrontation or consolidation, a finding explicitly frozen by an earlier pass becomes an operative premise of the next pass and may be reclassified only when a demonstrable factual contradiction or a material element previously unavailable is identified and cited.

The experimental 0.7.0 development branch was never released as the next stable wrapper. Its publication-specific work was separated from the public generic wrapper before 1.0.0.

## Tested and validated hosts

Revision 0.4.2 received the documented cross-host smoke test with ChatGPT 5.6 and Claude Opus 5.

Revision 0.5.0 was validated as a non-regressive wrapper migration targeting V5.0.0.

Revision 0.6.0 was structurally validated for V5.1.0, and its final portable ZIP was successfully imported by Claude.

Version 1.0.0 was produced by controlled migration from the complete stable wrapper lineage, structurally validated, repackaged reproducibly, checked by reverse migration against its release-candidate baseline, and subjected to acceptance/non-regression tests. These checks validate the package and execution safeguards; they do not imply identical analytical performance across hosts.

Execution quality still depends on the host environment: effective context, output capacity, document ingestion, access to external sources, and persistence of instructions over a long execution.
