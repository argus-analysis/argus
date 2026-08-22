# Versioning

ARGUS has two independent version lines.

## Protocol

The protocol uses versions such as **V5.0.0**. A protocol version identifies the normative analytical method.

Current stable protocol: **ARGUS V5.0.0**.

## Skill wrapper

The execution wrapper uses versions such as **0.4.3**. A wrapper revision can correct host-facing execution, formatting, activation, or output behavior without changing the normative method.

Current stable wrapper: **ARGUS Skill 0.4.3**, targeting ARGUS V5.0.0.

A technical wrapper correction does not by itself create a new protocol version. Conversely, a change to the protocol may require a new wrapper revision.

Recommended Git tags:

- protocol releases: `protocol-v5.0.0`
- Skill releases: `skill-v0.4.3`
