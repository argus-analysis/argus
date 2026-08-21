---
name: argus
description: Apply ARGUS V5.0.0 (Analyse Rigoureuse Guidee par un protocole Universel et Systematique) to argumentative texts and related corpora. Use when the user explicitly asks to analyze, audit, critique, compare, cross-audit, or consolidate a text with ARGUS, ARGUS Light, an ARGUS appendix, or ARGUS-Corpus, including pasted text and attached documents. Also use for an ARGUS fidelity check when a secondary text explicitly relates to an available primary source. Do not invoke for an ordinary summary or critique unless ARGUS is requested.
---

# ARGUS

Apply the bundled ARGUS V5.0.0 protocol faithfully. Treat this skill as an execution wrapper around the published protocol, never as a replacement, abridgement, or reinterpretation of it.

**Wrapper revision:** 0.4.2. This revision targets ARGUS V5.0.0. The wrapper revision is technical and host-independent; it never changes an ARGUS conclusion.

## Authority and resources

Use the bundled resources in this order:

1. `references/argus-protocol-fr.md` — normative ARGUS V5.0.0 protocol. Never edit, abridge, reflow, or silently simplify it.
2. `references/execution-rules.md` — non-normative execution guidance for host/tool behavior and portable restitution.
3. `references/output-template-fr.md` — default French output structure.
4. `references/versions-fr.md` — published protocol versioning policy and history.

If wording differs, the protocol prevails. Never introduce a defect category, severity label, appendix, threshold, or output judgment absent from the protocol.

## Frontier between protocol and wrapper

Keep the wrapper operational only. A rule belongs in the protocol if removing it would change a reachable ARGUS finding, severity, appendix activation, or conclusion. A wrapper update may improve execution, tool use, portability, or formatting, but must not change the result ARGUS permits.

Declare both numbers in every full analysis header:

- ARGUS V5.0.0
- wrapper revision 0.4.2

## Execution workflow

1. **Identify mode and exact object.**
   - Use full ARGUS V5.0.0 when the user asks for ARGUS without requesting a shorter mode.
   - Use ARGUS Light only when the user requests Light or an explicitly shorter ARGUS analysis.
   - Record the exact object before reasoning: support, title, publication date, and any distinct edition/version signaled by the document.
   - Keep all external verification tied to that exact object.

2. **Run Step 0 before any substantive analysis.**
   - Perform the integrity check first.
   - Apply 0.a and 0.a bis exactly as written.
   - If relevance is partial, weak, null, or ambiguous, stop where the protocol requires and submit only the three elements prescribed by 0.a.
   - Preserve the two distinct exemption cases. A perimeter already fixed by the user is not the same as validation being waived without a user-fixed perimeter.
   - For strong relevance, still state and motivate the perimeter declaration required by 0.a bis.
   - In the rendered header, choose exactly one perimeter-status branch. Strong relevance uses only `perimeter equal to the full text -- [reason]`; never append the unilateral/no-validation formula. A user-fixed perimeter, a user-validated perimeter, and a validation waiver without a user-fixed perimeter are mutually exclusive branches for the same decision.

3. **Apply every step required by the selected mode.**
   - Never fill a difficult section with speculation merely to look complete.
   - Preserve the distinctions between insufficient evidence, exclusion from scope, analyst indecision, and a non-attributable absence.
   - Apply 3.E in its required order: first gate, then second gate. Do not use the second-gate criterion to refuse a first-gate strategic omission.
   - Before calling anything an absence in 3.E, confirm that the information is actually absent from the analyzed object. If the text mentions it even to dismiss, minimize, recode, or neutralize it, do not label it an omission; examine the treatment under the applicable contradiction, symmetry, or audience-adaptation rules instead.
   - Before qualifying an absence as strategic, name the concrete support, statement, dataset, or fact that made the missing information readily accessible at the publication date. Do not treat phrases such as `widely available`, `well known`, or `publicly documented` as proof by themselves. If establishing accessibility required an external search or source lookup, that lookup is a 3.B control and must be counted with its status. If accessibility at the relevant date is not established, use the protocol's non-determinable or non-imputable branch rather than asserting strategic omission.
   - Return explicitly to the 0.f audience hypothesis at the end of Step 3.

4. **Activate appendices only at their protocol-defined point.**
   - Appendix 2: decide after reconstructing the central thesis in Step 2. The boundary test controls automatic activation; record the decision even when negative.
   - Appendix 3: for a genuine corpus, activate it **before the first text**. Run its integrity/relevance triage and single validation before individual analyses, then apply the base protocol text by text and finish the corpus controls.
   - Appendix 4: activate for numerical material that is probative under its section 2 criterion, not only for numbers indispensable to the conclusion.
   - For Appendix 4 Test A, do not let a bare distance-versus-range comparison stand in for the protocol's order-of-magnitude impossibility logic. If there is no repeated-count/time-window/reference-set structure to which the protocol's non-repeatable-unit and bound conditions apply, do not manufacture one; evaluate the quantitative claim under the other applicable Appendix 4 tests and/or 3.B, and do not assert an impossibility from Test A.
   - In Light mode, preserve only Appendix 4 Tests A and G as specified by the protocol. Do not combine ARGUS Light with ARGUS-Corpus.
   - Every appendix declared active must produce its visible restitution.

5. **Perform external verification when ARGUS requires it.**
   - Use available search/web/document tools for decisive elements when a simple check can establish them.
   - Never present model memory as external verification.
   - Declare the two independent axes required by 3.B: control status and source-access mode.
   - Declare the three counts separately: completed, partial, unsuccessful controls. If completed controls are zero, justify zero.
   - Keep the unit of a control stable from the moment the verificative proposition is formulated; do not repartition it after seeing the result.
   - Apply verification symmetrically and report unsuccessful checks as unsuccessful, never as proof of falsity.
   - Apply the proportionality warning per individual object, not by mechanically summing a corpus.
   - If a required check cannot be executed in the current environment, state the limitation and do not claim the requirement was satisfied.

6. **Use the primary-source fidelity test only when its activation relation is established.**
   - A primary, official, contemporary, or relevant document does not activate the fidelity test by itself.
   - Establish that the analyzed text cites, names, summarizes, comments on, criticizes, or otherwise demonstrably reproduces that source.
   - Then apply the seven protocol qualifications to decisive claims only.
   - Do not convert an attached primary source into a corpus automatically.

7. **Produce the analysis in a portable form.**
   - Use `references/output-template-fr.md` by default for French output unless the user requests another language or format.
   - Preserve mandatory sections, especially 7.b and Step 8.
   - In 7.c reproduce all five levels 0-4 and keep level, rhetorical mode, and origin/function as separate fields.
   - Respect Rule 15: no Markdown or HTML tables.
   - For external checks, use portable plain-text source callouts `[S1]`, `[S2]`, etc., resolved in a terminal source list. Do not rely solely on host-native citation rendering in an artifact meant to be exported or archived.

8. **Run Step 8 as a correction pass before delivery.**
   - Correct inconsistencies rather than merely listing them.
   - Check appendix declarations, all three verification counts, calculations, factual consistency, primary-source activation, and absence qualification.
   - Apply Rule 19 to the analysis itself.
   - Answer deference and serial-conformism items with a precise case or an explicit statement that no case was identified.
   - Run the terminal reference-integrity check in `references/execution-rules.md`.
   - Run a mechanical Rule 15 pass over Markdown list items. Treat this as a pass/fail delivery gate: outside fenced code blocks, the final Markdown must contain zero list-item lines matching `^\s*[\*\+] `. Replace every such marker with `- ` before delivery. Do not alter emphasis, block quotes, code, or numbered lists.

## Corpus behavior

For a related corpus, keep each text as its own ARGUS object. Execute C.1 and C.1 bis before the first individual analysis. Then analyze each retained text under the base protocol and finish C.3-C.6 as required.

Do not let long-output pressure silently compress the later texts. When a corpus is too large for one reliable response, segment the delivery explicitly while preserving the protocol order and the shared corpus state. Never merge protocol steps to save space.

For several unrelated texts, analyze them separately and compare only after the individual analyses unless the user explicitly defines a different task.

## Reliability and contradiction

Treat ARGUS as an aid to critical reading, not a measurement instrument. Preserve the protocol's reliability notice and do not hide model uncertainty.

For contradiction or cross-audit requests, follow the protocol's three levels. A genuine blind cross-audit must not be contaminated by the first analysis. When consolidating two independent analyses, do not average them: separate convergence, divergence, coverage divergence, disagreement type, insufficiency-vs-conclusion cases, and what would resolve each divergence.

## Host-capability rule

A full ARGUS run requires enough effective context, output capacity, documentary ingestion, and instruction persistence to complete the protocol faithfully. If the environment cannot maintain the required state or output, say that the run cannot be represented as a complete ARGUS execution. Offer ARGUS Light, a reduced corpus, or another execution strategy rather than silently truncating or omitting steps.

## Final quality check

Before delivery, verify:

- exact object and publication date declared;
- correct ARGUS version, mode, and wrapper revision declared;
- integrity and relevance logic executed in the correct order;
- perimeter status and reason declared;
- appendix decisions taken at the right point and every activated appendix visibly restituted;
- return to 0.f present at the end of Step 3;
- three external-control counts and their subjects consistent with the body;
- no remembered fact mislabeled as externally verified;
- primary-source fidelity test activated only when filiation is established;
- 3.E first and second gates applied in order; every claimed absence is actually absent, and every strategic-omission accessibility claim names its date-relevant support and corresponding 3.B control when externally checked;
- 7.c contains five levels and keeps descriptors separate from the level;
- 7.b is substantive and Step 8 is present;
- Step 8 corrected all correctable inconsistencies;
- no table appears anywhere;
- Rule 15 terminal gate passed: outside fenced code blocks, zero list-item lines match `^\s*[\*\+] ` and every Markdown bullet list uses `- `;
- portable references resolve and no placeholder or broken citation marker remains;
- no category, threshold, severity, or rule absent from ARGUS V5.0.0 has been invented by the wrapper.
