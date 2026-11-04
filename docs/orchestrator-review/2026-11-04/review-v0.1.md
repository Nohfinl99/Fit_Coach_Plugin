# Independent review — Fit_Coach rebuild proposal v0.1

**Reviewed artifact:** `proposal.md`  
**SHA-256:** `E3C862437304B4459EEE2D9FE9E51C7BCE6851891BCB1488B627608897FF69A1`  
**Reviewer:** GPT-6 Astra, high reasoning, separate session; requested as Evidence-Synthesizer review  
**Review type:** document red-team only; no product code, model run, benchmark, or pilot reviewed

## Decision

**GO** for the read-only source baseline and proposal/design work. **NO-GO** for implementation, benchmark execution, pilot, or release until the issues below and their gates are resolved. No Critical finding was identified within this document-only scope; that does not certify the unrun product.

## Findings

### High

1. **Host and validator not selected.** The draft promised a deterministic validator although the current product is described as a prompt/plugin package. Choose whether V1 remains a prompt-only plugin with an external evaluation harness or becomes a host-integrated application. Mark validator `PROPOSED_NOT_IMPLEMENTED`; restrict deterministic claims to encoded schema/arithmetic/constraints.
2. **Execution path absent from the DAG.** The draft went from a rewrite proposal to R4b without candidate implementation, independent R4a, executor, raw capture, or budget. Add each step with pinned inputs, acceptance, owner, budget, and stop conditions.
3. **Rubric was not repeatable or decision-ready.** Terms such as “plausible” and “coherent” lacked scoring anchors; applicability, N/A, missing outputs, false refusals, and thresholds were undefined. Define anchors and positive/negative examples, applicable denominator, refusal handling, critical failures, and freeze thresholds before seeing results. Three runs per case are only an initial variance check.

### Medium

4. **Vietnamese-context rule was anti-stereotyping but its applicability plan was thin.** WHO STEPS is population risk surveillance, not proof that a particular hypertrophy dose works for Vietnamese people. Map each evidence population to decisions it can support; keep unsupported population-specific exercise response `UNKNOWN`; test diverse Vietnamese profiles and use the user's own measurements/logs for personalization.
5. **Community reports had not actually been reviewed.** Add a scoped community-source scan with community, thread/report, date, selection method, population, and bias. Use community material for experience/usability; confirm physiology claims against research. Do not call a handful of posts representative.
6. **Benchmark size and reviewer calibration lacked a budget.** Start with a small coach-calibration set and adjudicated examples before expanding. Match context/output limits across baselines; separate development, calibration, held-out, and AI-judge-validation cases.
7. **User log privacy was unspecified.** Define data location, minimum fields, access, export/correction/deletion, and host/model transmission before collecting real logs. Public fixtures must be synthetic or appropriately de-identified.

### Low

8. Use `FC-*` task IDs to avoid collisions with Orchestrator's existing A0–A7 coverage labels; keep the user-facing proposal in Vietnamese; state read depth per evidence source (search result, abstract, selected sections, or full text).

## Revision disposition

The v0.2 draft was created as a new revision, preserving v0.1 and this review record. It adds host/evaluation-harness boundaries, explicit R4a/execution/R4b stages, rubric anchors and refusal/N/A treatment, community-scan limitations, Vietnam evidence applicability, and profile/log privacy. v0.2 still requires exact-digest review before use as a frozen plan.
