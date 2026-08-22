# ARGUS Protocol

**ARGUS** — *Analytical Rigor Guided by a Universal and Systematic protocol* — is an open protocol for the critical analysis of argumentative texts with the assistance of artificial intelligence.

- **Current protocol:** ARGUS V5.0.0
- **Current Skill wrapper:** ARGUS Skill 0.4.3
- **Website:** https://www.argus-protocol.org
- **Repository:** https://github.com/argus-analysis/argus
- **Author:** François Vadrot

The protocol and the Skill use **separate version numbers**. The Skill is an execution layer that makes the protocol easier to invoke on compatible platforms; it does not replace or redefine the protocol. **ARGUS V5.0.0 remains the normative reference.**

## Protocol V5.0.0

The protocol is available here in six languages:

| Language | Source |
|---|---|
| Français | [argus-protocol-fr.md](protocol/V5.0.0/argus-protocol-fr.md) |
| English | [argus-protocol-en.md](protocol/V5.0.0/argus-protocol-en.md) |
| Español | [argus-protocol-es.md](protocol/V5.0.0/argus-protocol-es.md) |
| Deutsch | [argus-protocol-de.md](protocol/V5.0.0/argus-protocol-de.md) |
| Italiano | [argus-protocol-it.md](protocol/V5.0.0/argus-protocol-it.md) |
| Português | [argus-protocol-pt.md](protocol/V5.0.0/argus-protocol-pt.md) |

The French source is the normative source bundled in the current Skill wrapper. The published translations reproduce the same V5.0.0 protocol for use in their respective languages.

## ARGUS Skill 0.4.3

The stable wrapper for ARGUS V5.0.0 is in [`skill/V0.4.3`](skill/V0.4.3/).

It contains:

- the installable archive [`argus-0.4.3.zip`](skill/V0.4.3/argus-0.4.3.zip);
- the unpacked Skill source under [`skill/V0.4.3/argus`](skill/V0.4.3/argus/);
- the normative French V5.0.0 protocol and versioning reference bundled by the Skill;
- technical execution rules and an output template.

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

- ARGUS V5.0.0 normative French source: `4da638b15145c5f13183cf5d9e6b9dfb4f503b425ba3f576eded8c9aed53ca85`
- ARGUS Skill 0.4.3 ZIP: `a5d7b0bffeaff1717e6b58fafff1bf91cd68fdcc68eafc02aa9196af0c752f60`

## Versioning

Protocol versions and Skill wrapper revisions evolve independently. See [Versioning](docs/versioning.md).

This public repository starts with **ARGUS V5.0.0** and **ARGUS Skill 0.4.2**. Earlier protocol history remains documented on the ARGUS website.

## Licence

The ARGUS Protocol is published under **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**. See [LICENSE.md](LICENSE.md) and the licence page on the ARGUS website.
