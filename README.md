# ARGUS Protocol

**ARGUS** — *Analytical Rigor Guided by a Universal and Systematic protocol* — is an open protocol for the critical analysis of argumentative texts with the assistance of artificial intelligence.

- **Current protocol:** ARGUS V5.1.0
- **Current Skill wrapper:** ARGUS Skill 1.0.0
- **Website:** https://www.argus-protocol.org
- **Repository:** https://github.com/argus-analysis/argus
- **Author:** François Vadrot

The protocol and the Skill use **separate version numbers**. The Skill is an execution layer that makes the protocol easier to invoke on compatible platforms; it does not replace or redefine the protocol. **ARGUS V5.1.0 remains the normative reference.**

## Protocol V5.1.0

The protocol is available here in six languages:

| Language | Source |
|---|---|
| Français | [argus-protocol-fr.md](protocol/V5.1.0/argus-protocol-fr.md) |
| English | [argus-protocol-en.md](protocol/V5.1.0/argus-protocol-en.md) |
| Español | [argus-protocol-es.md](protocol/V5.1.0/argus-protocol-es.md) |
| Deutsch | [argus-protocol-de.md](protocol/V5.1.0/argus-protocol-de.md) |
| Italiano | [argus-protocol-it.md](protocol/V5.1.0/argus-protocol-it.md) |
| Português | [argus-protocol-pt.md](protocol/V5.1.0/argus-protocol-pt.md) |

The French source is normative. The five published translations are audited V5.1.0 translations for use in their respective languages.

V5.1.0 adds the **modal constancy control**, a directional test for modal retraction: the same load-bearing proposition being asserted strongly where it performs argumentative work and weakened where strong commitment would carry a cost. It leaves the existing categories, thresholds, proof standard and overall procedure of V5.0.0 unchanged.

## ARGUS Skill 1.0.0

The stable wrapper for ARGUS V5.1.0 is in [`skill/V1.0.0`](skill/V1.0.0/).

It contains:

- the installable archive [`argus-wrapper-v1.0.0.zip`](skill/V1.0.0/argus-wrapper-v1.0.0.zip);
- the unpacked Skill source under [`skill/V1.0.0/argus`](skill/V1.0.0/argus/);
- the normative French V5.1.0 protocol and versioning reference bundled by the Skill;
- technical execution rules and an output template;
- a dedicated wrapper version history.

Version 1.0.0 is the first stabilized public boundary of the **generic ARGUS execution wrapper**. It keeps the wrapper independent of any website or downstream publication workflow. Publication-specific Case Study and editorial-pipeline conventions are outside the public wrapper and belong in separate tooling.

The 1.0.0 hardening also requires Step 8 corrections to propagate into the final Step 7.c judgment, makes the Level 2 / Level 3 boundary explicit in terms of effective convergence rather than defect accumulation, and preserves explicitly frozen findings across multi-pass adjudication unless a new material element is identified.

The experimental 0.7.0 development branch was never published as the next stable wrapper; its publication-specific work was separated before 1.0.0.

Minimal use after installation:

> Analyze this text with ARGUS.

For a shorter execution:

> Analyze this text with ARGUS Light.

For related texts:

> Analyze these texts as a corpus with ARGUS.

See [Using the ARGUS Skill](docs/skill.md) for details and known limitations.

## Integrity and checksums

Repository release files are hashed in [`CHECKSUMS.sha256`](CHECKSUMS.sha256).

Key published hashes:

- ARGUS V5.1.0 normative French source: `4d4929996358cd1359d0349c3cee93c8e54d39a4ca5f3143861b2bff8dc7feee`
- ARGUS Skill 1.0.0 ZIP: `8e48404edfc95371191825ca77a06c5ce7b62dba71aa85aff415dd2e6a321cef`

## Versioning

Protocol versions and Skill wrapper revisions evolve independently. See [Versioning](docs/versioning.md).

The repository preserves earlier stable releases under `protocol/` and `skill/`; the current stable pair is **ARGUS V5.1.0 / ARGUS Skill 1.0.0**.

## Licence

The ARGUS Protocol is published under **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**. See [LICENSE.md](LICENSE.md) and the licence page on the ARGUS website.
