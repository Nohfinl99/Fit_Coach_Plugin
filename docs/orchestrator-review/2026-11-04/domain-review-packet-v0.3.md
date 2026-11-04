# Fit_Coach domain review packet v0.3

**Status:** DRAFT v0.3 / prepared for qualified-human review / NOT_SENT  
**Prepared:** 2026-11-02  
**Supersedes:** v0.2 (retained as review history; clarifies retention of CB-11 after independent logic review).  
**Purpose:** Obtain domain review needed for FC-03 acceptance. This packet does not approve claims, close a product gate, authorize model execution, or change the GitHub product source.

## 1. Review target and limits

- **Product source:** `Nohfinl99/Fit_Coach_Plugin`, baseline commit `06f7558b327068c414d252528741d0918e141cbc`.
- **Pinned package evidence:** `source-baseline-2026-11-02.json`; exact content hashes are recorded there. Review the four canonical references and `plugin.json` at that revision, not the preview ZIP note as runtime behavior.
- **Current product state:** GitHub PR [`#1`](https://github.com/Nohfinl99/Fit_Coach_Plugin/pull/1) was observed read-only on 2026-11-02 as OPEN, base `main`, head `codex/fit-coach-preview-2026-11-02` at `b6970cebff3c17fbad32a66a51ae8ac9ae8aa7ed`, 3 files, no conflicts, no checks and no reviews at observation time. It contains a review-preview archive of the unchanged source snapshot; it is not a rebuilt or validated release. This is a dated observation and may drift. The active skill does not enforce the Vietnamese-nationality guardrail; that statement is currently only in the ZIP note.
- **Exact evidence inputs (SHA-256):** `proposal-v1.0.md` `BA901F24DD20359CEA04F93F2969D7C222B189FF203C5CF9D937D1A60506A0A4`; `claim-evidence-audit-v0.2.md` `38578471898493FE5E5CFFEC7DA3DE79A72709BB889ED6F067C0B0C9D2723DDF`; `evidence-update-2026-11-02-v0.3.md` `7F39ABD5A2CCB6983E3697DD9D93D9390644418F8EF81E141593DB4368310873`; `calibration-benchmark-v0.4.md` `98369C6F284DC6F27601CB80709C91E9512A8A02C925E0B441D702F3528EC92F`. These are desk research/design artifacts. They are not expert approval or actual-host results.
- **Execution:** product benchmark, model calls, user pilot, and host upload remain `NOT_RUN`.

Reviewers should mark each item `APPROVE`, `REVISE`, `REMOVE`, or `OUT_OF_SCOPE`, with exact source locator, proposed allowed use, population/setting, rationale, confidence/limitations, reviewer qualification, date, and conflict disclosure. If source depth is inadequate, mark `NEEDS_SOURCE_REVIEW`; do not infer approval from silence.

## 2. Required reviewers

### A. Resistance-training programming

At least two independent, currently qualified strength/resistance-training coaches should review V1 exercise programming and calibration anchors. Record relevant credential, issuing body, current status, practical scope, and conflict of interest. A third qualified coach adjudicates material disagreements; keep each original rating.

### B. Acute symptoms and musculoskeletal safety

Use a currently licensed medical professional whose scope includes acute exercise-related red flags for chest pain, dizziness, fainting, and breathing symptoms. Use a suitably qualified clinician with musculoskeletal expertise for pain/injury escalation language. Do not ask either reviewer to approve diagnosis or rehabilitation content; those are outside V1.

The medical reviewer must also assess acute-risk boundaries for rapid weight-cut/dehydration requests, coordinated with the nutrition review where relevant.

### C. Nutrition and supplements

Use a currently credentialed dietitian or qualified sports-nutrition professional for any food, nutrition, or supplement content retained. If this review is unavailable, remove food/nutrition/supplement content and nutrition-advice benchmark cases from V1; do not retain nutrition education based only on AI/source review. Keep CB-11 as a medical-reviewed safety/refusal-boundary case even if nutrition content is removed. Rapid weight cuts, dehydration, diuretics, and peak-week manipulation remain excluded and need appropriate acute-risk review.

## 3. Review assignments

| Review area | Source locator / design IDs | Questions to resolve | Required result |
|---|---|---|---|
| Programming claims | Claim audit CA-01–CA-10d; protocol IDs PR-VOL, PR-INT, PR-PRG, PR-FRQ, PR-RST; ontology K04 | Which legacy numeric thresholds or fixed intervals must be removed, quarantined, or retained only as explicitly provisional examples? What conservative programming choices are acceptable for healthy adults when profile data are sufficient? Which cues/progression rules require clarification? | Item-level disposition; prohibited wording; any eligible provisional example ranges plus their conditions, evidence limits, and monitoring rules. |
| Evidence routing and conflicting legacy content | CA-11; benchmark CB-08, CB-14, CB-16–CB-21, CB-25 | Does the proposed `IMPORTED_UNVERIFIED` handling prevent a legacy claim from driving individualized advice when it conflicts with the overlay? Are the cases and failure labels clinically/coaching meaningful? | Required use-deny rules, case edits, and any additional conflict probes. |
| Vietnamese localization | CA-12; CB-01, CB-09, CB-22A/B, CB-23, CB-24 | Are language, kg/cm, equipment/access and familiar examples appropriate? Is the matched nationality test fair? Can any proposed statement be misread as a single Vietnamese body type or dose? | Localization revisions and explicit confirmation that no physiological inference is justified by nationality alone. |
| Acute red flags / pain | SAFE-01/02 and CB-06/07; safety redlines in benchmark v0.4 | Are immediate actions and escalation language correct and proportionate in Viet Nam? Does the case distinguish emergency symptoms, persistent pain, urgent warning signs, and ordinary discomfort without diagnosing? | Exact approved action language and critical redlines; source locators; scope and limitations. |
| Rapid weight-cut boundary | SAFE-03 and CB-11 | Are refusal and acute-risk referral boundaries safe and proportionate? Is the requested behavior clear without giving actionable dehydration, diuretic, or peak-week manipulation steps? | Exact refusal/redirect language and redlines; coordinate with nutrition reviewer. |
| Nutrition/supplements | CA-13; CB-10 and any other nutrition/supplement benchmark cases | Should these items be removed from V1, or can specific claims be retained after both qualified nutrition review and a separate claim-level source audit? | Item-level scope decision. If qualified review is unavailable, remove nutrition content and related nutrition-advice cases; retain CB-11 for medical-reviewed safety/refusal behavior. No personalized numeric protocol may remain by default. |
| Rubric/calibration anchors | Eight dimensions and 0/1/2 anchors in benchmark v0.4; CB-01–CB-25 | Are anchors observable, fair, applicable to the stated case, and free of one-plan gold-standard bias? Are case applicability, safety redlines, false-refusal labels, and disagreement/adjudication rules clear? | Independent anchor ratings and case-specific positive/negative examples before any R4a freeze. |

## 4. Vietnamese population rule

The target context is Vietnamese language and user-relevant environment: metric units, user-selected foods, schedule, equipment, cost/access, and locally applicable evidence. Nationality is not an individual physiological measurement. Do not infer a user's body composition, metabolism, strength, recovery, injury risk, or training dose from being Vietnamese or Asian. The available Vietnamese intervention cited in the evidence update is limited to older adults with sarcopenia and a small cluster design; it does not justify a population-wide gym prescription. Ask for relevant individual data and use the person's observed response.

This is a product requirement for reviewer scrutiny. It is not currently enforced by the active SKILL.md and must not be represented as an existing runtime safeguard.

## 5. Decision and records

The FC-03 owner records:

1. Each reviewer's qualification, scope, conflicts, exact source revision reviewed, and date.
2. Independent ratings before discussion; disagreements and adjudication separately.
3. Exact claim/case locator, disposition, allowed wording, population limits, and evidence needed for any unresolved item.
4. Accepted V1 scope, host/workflow, output schema, privacy/data handling statement, safety boundaries, claim map, provisional rubric anchors, and acceptance criteria.
5. An updated exact-digest FC-03 specification and an independent high-capability logic review. High-model review is not domain approval.

Until these records exist, status remains `FC-03 INCOMPLETE`. A reviewer response alone does not authorize a run: calibration R4a requires accepted FC-03, an FC-04 local candidate revision and diff-intent report, and separate independent review under the proposal DAG. No calibration R4a, model run, pilot, merge-as-release, or product release is authorized by this packet. A reviewer response may narrow V1 or recommend removal of an entire content area. Preserve the old source and prior FAIL/history; any accepted product change must be a new revision with a diff-intent record.

## 6. Handoff request

**Requested from product owner:** nominate or engage the qualified reviewers above, or identify a permitted review route and budget. The packet is prepared but has not been sent to anyone. No third party has been contacted.

**Next atomic task after reviewer responses:** Product-Evolution-Architect consolidates only the received, attributable domain decisions into FC-03 v1.1, leaves unresolved claims explicitly unresolved, obtains exact-digest independent review, and presents the FC-03 acceptance decision. Only after FC-03 acceptance may Prompt-Master begin FC-04; calibration R4a remains blocked until FC-04 and its independent review are also complete. Do not skip these gates.


## v0.3 review fixes

- Separated CB-11 (rapid weight cut) from acute symptom/pain cases CB-06/07 and assigned acute-risk/nutrition review as applicable.
- Made qualified nutrition review mandatory for any retained nutrition content; otherwise remove the content and cases from V1.
- Added exact digests for every cited proposal/audit/evidence/benchmark input and a dated PR #1 observation.
- Named accepted FC-03, FC-04 local candidate, and independent review as prerequisites to calibration R4a.
- Clarified that CB-11 remains a medical-reviewed safety/refusal case if nutrition education and nutrition-advice cases are removed.


