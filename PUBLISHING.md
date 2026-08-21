# First GitHub publication

Organization: `argus-analysis`

Repository name: `argus`

## 1. Create the repository

Create an empty public GitHub repository named `argus` in the `argus-analysis` organization. Do not initialize it with another README or licence if you are uploading this prepared tree as-is.

## 2. Publish this tree

Upload or push the complete contents of this repository root.

Suggested initial commit message:

`Publish ARGUS V5.0.0 and Skill 0.4.2`

Suggested repository description:

`Open protocol for AI-assisted critical analysis of argumentative texts. ARGUS V5.0.0 · Skill 0.4.2.`

Suggested website field:

`https://www.argus-protocol.org`

## 3. Create the protocol release

Tag: `protocol-v5.0.0`  
Title: `ARGUS Protocol V5.0.0`

Use `releases/protocol-v5.0.0.md` as the release description.

Prepared release asset:

`ARGUS-Protocol-V5.0.0-Markdown.zip`

## 4. Create the Skill release

Tag: `skill-v0.4.2`  
Title: `ARGUS Skill 0.4.2`

Use `releases/skill-v0.4.2.md` as the release description.

Prepared release asset:

`argus-0.4.2.zip`

The Skill ZIP must retain this SHA-256:

`43a274de86f983d07eabbdb2387f7cbb4b3bb870e1a858258b6e02bfaad64edf`

## 5. Git command equivalent

After creating the empty remote repository:

```bash
git init
git add .
git commit -m "Publish ARGUS V5.0.0 and Skill 0.4.2"
git branch -M main
git remote add origin https://github.com/argus-analysis/argus.git
git push -u origin main

git tag -a protocol-v5.0.0 -m "ARGUS Protocol V5.0.0"
git tag -a skill-v0.4.2 -m "ARGUS Skill 0.4.2"
git push origin protocol-v5.0.0 skill-v0.4.2
```

Create the two GitHub Releases from those tags and attach the corresponding prepared asset.
