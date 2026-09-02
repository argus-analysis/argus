# Publishing ARGUS releases

- Organization: `argus-analysis`
- Repository: `argus`

The protocol and the Skill wrapper have independent version lines and therefore use separate tags and separate GitHub Releases.

## 1. Prepare repository contents

For a protocol release `Vx.y.z`:

- add the six audited protocol Markdown files under `protocol/Vx.y.z/`;
- add `releases/protocol-vx.y.z.md`;
- update the current-version references in `README.md`, `README.fr.md`, `CHANGELOG.md`, `CITATION.cff` and `docs/versioning.md` as appropriate;
- create the six-language release archive `ARGUS-Protocol-Vx.y.z-Markdown.zip` and its `.sha256` file.

For a Skill release `a.b.c`:

- add the unpacked canonical package under `skill/Va.b.c/argus/`;
- add the exact validated ZIP under `skill/Va.b.c/`;
- add `releases/skill-va.b.c.md`;
- update `README.md`, `README.fr.md`, `CHANGELOG.md`, `docs/skill.md` and `docs/versioning.md` as appropriate;
- publish the same validated ZIP as the GitHub Release asset, together with its `.sha256` file.

Regenerate `CHECKSUMS.sha256` after all repository files have reached their final content.

## 2. Review before publishing

Before any remote write:

- verify the canonical protocol and wrapper hashes;
- verify that the wrapper-embedded normative protocol is byte-identical to the published normative French source;
- inspect the complete Git diff;
- confirm that older protocol and Skill directories remain unchanged;
- confirm that release ZIP entry names use portable `/` separators.

## 3. Commit and merge

Prepare releases on a dedicated branch, for example:

`release/v5.1.0-wrapper-0.6.0`

Use one atomic repository commit when the protocol and wrapper are being published as a coordinated stable pair. Merge that commit to `main` after review.

## 4. Tags

Protocol tags use:

`protocol-vx.y.z`

Skill tags use:

`skill-va.b.c`

Tags should point to the reviewed release commit on `main`.

## 5. GitHub Releases

Create two GitHub Releases when a protocol and wrapper are published together:

- **ARGUS Protocol Vx.y.z** â€” body from `releases/protocol-vx.y.z.md`; attach the protocol Markdown ZIP and `.sha256`.
- **ARGUS Skill a.b.c** â€” body from `releases/skill-va.b.c.md`; attach the exact validated wrapper ZIP and `.sha256`.

Never rebuild the wrapper ZIP during GitHub publication: the release asset must be the same canonical archive that was validated before publication.

## Current stable pair

- Protocol: ARGUS V5.1.0
- Skill wrapper: ARGUS Skill 0.6.0
- Website: https://www.argus-protocol.org
