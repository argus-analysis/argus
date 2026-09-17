# Versioning

ARGUS has two independent version lines.

## Protocol

The protocol uses versions such as **V5.1.0**. A protocol version identifies the normative analytical method.

Current stable protocol: **ARGUS V5.1.0**.

A minor protocol version adds a test, section or appendix without changing the existing categories, thresholds or evaluation method for mechanisms already covered by the previous version. V5.1.0 is such a minor release: it adds modal constancy control while leaving the V5.0.0 evaluation framework intact.

## Skill wrapper

The execution wrapper uses versions such as **1.0.0**. A wrapper revision can correct host-facing execution, formatting, activation, provenance or output behaviour without independently changing the normative method.

Current stable wrapper: **ARGUS Skill 1.0.0**, targeting ARGUS V5.1.0.

Version 1.0.0 establishes the stable public boundary of the **generic execution wrapper**. Site-specific publication, Case Study and editorial-pipeline conventions are not part of that public wrapper and must be handled by separate tooling.

The 0.7.0 line was a development branch used to experiment with publication-specific orchestration. It was never released as the stable successor to 0.6.0; its publication-specific work was separated before 1.0.0.

A technical wrapper correction does not by itself create a new protocol version. Conversely, a protocol change may require a new wrapper revision.

Recommended Git tags:

- protocol releases: `protocol-v5.1.0`
- Skill releases: `skill-v1.0.0`
