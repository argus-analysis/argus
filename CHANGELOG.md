# Changelog

This GitHub repository begins with the current stable public state of ARGUS. Earlier protocol history is documented on https://www.argus-protocol.org.

## 2026-08-26 — ARGUS Skill 0.5.0

- Controlled migration from Skill 0.4.3 targeting ARGUS V5.0.0; the normative protocol is unchanged.
- Clarifies neutral input: ARGUS does not require a user-supplied analytical question, hypothesis or prior orientation.
- Adds execution metadata for model, host and execution regime.
- Distinguishes wrapper execution from context-only execution.
- Adds publication-layer rules for ARGUS Case Studies without creating a new analytical mode.
- Adds a dedicated wrapper version history.
- Migration passed the complete non-regression control set and final independent audit.

## 2026-08-22 — ARGUS Skill 0.4.3

- Technical portability update targeting ARGUS V5.0.0; the normative protocol is unchanged.
- External source references use Markdown links such as `[S1](URL)` when a usable URL is available, while retaining plain `[S1]` for supplied pieces without a URL.
- The output header can preserve the original or canonical URL of the analyzed object when it is explicitly available.
- Terminal checks now verify portable source links and analyzed-object URLs before delivery.
- The packaged Skill passed structural validation before publication.

## 2026-08-21 — ARGUS Protocol V5.0.0

- Stable V5.0.0 protocol published in six languages.
- Normative French source frozen and checksummed.
- Protocol execution requirements expressed in terms of effective context, output capacity, document ingestion and persistence of instructions rather than a fixed token threshold.
- Corpus, primary-source fidelity, external verification, omission analysis, interpretive-closure classification and quantitative-control rules consolidated in the stable V5 line.

## 2026-08-21 — ARGUS Skill 0.4.2

- Stable execution wrapper targeting ARGUS V5.0.0.
- Wrapper/protocol versioning kept separate.
- Final corrections harden scope handling, Appendix 4 Test A activation and Step 3.E omission controls.
- Tested with ChatGPT 5.6 and Claude Opus 5.
- Known non-substantive limitation: ChatGPT 5.6 may render some Markdown bullet lists with a marker other than the protocol-preferred hyphen.
