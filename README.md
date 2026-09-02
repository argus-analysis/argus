# ARGUS Protocol

**ARGUS** â€” *Analytical Rigor Guided by a Universal and Systematic protocol* â€” is an open protocol for the critical analysis of argumentative texts with the assistance of artificial intelligence.

- **Current protocol:** ARGUS V5.1.0
- **Current Skill wrapper:** ARGUS Skill 0.6.0
- **Website:** https://www.argus-protocol.org
- **Repository:** https://github.com/argus-analysis/argus
- **Author:** FranÃ§ois Vadrot

The protocol and the Skill use **separate version numbers**. The Skill is an execution layer that makes the protocol easier to invoke on compatible platforms; it does not replace or redefine the protocol. **ARGUS V5.1.0 remains the normative reference.**

## Protocol V5.1.0

The protocol is available here in six languages:

| Language | Source |
|---|---|
| FranÃ§ais | [argus-protocol-fr.md](protocol/V5.1.0/argus-protocol-fr.md) |
| English | [argus-protocol-en.md](protocol/V5.1.0/argus-protocol-en.md) |
| EspaÃ±ol | [argus-protocol-es.md](protocol/V5.1.0/argus-protocol-es.md) |
| Deutsch | [argus-protocol-de.md](protocol/V5.1.0/argus-protocol-de.md) |
| Italiano | [argus-protocol-it.md](protocol/V5.1.0/argus-protocol-it.md) |
| PortuguÃªs | [argus-protocol-pt.md](protocol/V5.1.0/argus-protocol-pt.md) |

The French source is normative. The five published translations are audited V5.1.0 translations for use in their respective languages.

V5.1.0 adds the **modal constancy control**, a directional test for modal retraction: the same load-bearing proposition being asserted strongly where it performs argumentative work and weakened where strong commitment would carry a cost. It leaves the existing categories, thresholds, proof standard and overall procedure of V5.0.0 unchanged.

## ARGUS Skill 0.6.0

The stable wrapper for ARGUS V5.1.0 is in [`skill/V0.6.0`](skill/V0.6.0/).

It contains:

- the installable archive [`argus-wrapper-v0.6.0.zip`](skill/V0.6.0/argus-wrapper-v0.6.0.zip);
- the unpacked Skill source under [`skill/V0.6.0/argus`](skill/V0.6.0/argus/);
- the normative French V5.1.0 protocol and versioning reference bundled by the Skill;
- technical execution rules and an output template;
- a dedicated wrapper version history.

Revision 0.6.0 updates the target to V5.1.0 and formalizes analyst provenance through model, version/build and provider-labelled reasoning intensity, while retaining host and execution-regime metadata.

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
- ARGUS Skill 0.6.0 ZIP: `949a375fc3a52b1c402e4026e843cb58a2a5d935253cf4fb3da6324f170ce817`

## Versioning

Protocol versions and Skill wrapper revisions evolve independently. See [Versioning](docs/versioning.md).

The repository preserves earlier stable releases under `protocol/` and `skill/`; the current stable pair is **ARGUS V5.1.0 / ARGUS Skill 0.6.0**.

## Licence

The ARGUS Protocol is published under **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**. See [LICENSE.md](LICENSE.md) and the licence page on the ARGUS website.
