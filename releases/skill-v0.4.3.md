# ARGUS Skill 0.4.3

**Release date:** 2026-08-22  
**Target protocol:** ARGUS V5.0.0  
**Status:** stable

ARGUS Skill 0.4.3 is the stable execution wrapper for ARGUS Protocol V5.0.0.

The Skill does not replace the protocol. ARGUS V5.0.0 remains the normative reference and is unchanged in this release.

## Changes in 0.4.3

- External verification references use Markdown links such as `[S1](URL)` whenever a usable URL is available.
- Supplied documents without a URL continue to use plain `[S1]` references with their document location in the terminal source list.
- The analysis header can preserve the original or canonical URL of the analyzed object when it is explicitly available.
- Terminal reference checks now include source-link integrity and analyzed-object URL preservation.

## Validation

The complete Skill package passed the structural validator before publication. Revision 0.4.2 remains the latest revision that received the documented cross-host smoke test with ChatGPT 5.6 and Claude Opus 5; 0.4.3 changes only the technical portability and restitution layer.

## Download integrity

`argus-0.4.3.zip`

File size: 75,339 bytes

SHA-256:

`a5d7b0bffeaff1717e6b58fafff1bf91cd68fdcc68eafc02aa9196af0c752f60`
