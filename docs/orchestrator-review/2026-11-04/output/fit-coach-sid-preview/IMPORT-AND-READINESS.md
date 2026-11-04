# Fit_Coach SID — GPT/agent import preview

Status: REVIEW PREVIEW, not an approved fitness product release.
Source snapshot: Nohfinl99/Fit_Coach_Plugin at commit `06f7558b327068c414d252528741d0918e141cbc` (2026-11-02 local baseline).

## Import

This archive contains the `fit-coach-sid/` plugin directory at the ZIP root, including `plugin.json`, the `fit-coach` skill, and its four references. Import support depends on the target ChatGPT/agent surface and its current upload UI. The manifest uses the third-party `agent-plugins.org` schema; this archive has not been confirmed as accepted by every ChatGPT plugin importer. If the upload flow rejects the ZIP, use `skills/fit-coach/SKILL.md` as the instruction entry point and upload the four `references/*.md` files as knowledge resources, where supported.

## Readiness limits

- This is an unchanged snapshot, repackaged for review; no coaching claims or runtime behavior were rebuilt in this ZIP.
- The fitness-domain gate is still open: qualified strength-coach review, medical review of red-flag cases, and nutrition review of retained nutrition content are not recorded.
- No host/model benchmark, user pilot, or product outcome validation has been run. Benchmark content is not evidence that the product passed.
- Imported protocol claims may remain `IMPORTED_UNVERIFIED`; do not treat this bundle as validated personalized numeric training or nutrition advice.
- Vietnamese localization means language, units, context and user-level personalization. It does not support inferring physiology or training dose from nationality. This guardrail is only stated in this archive note; the unchanged active SKILL.md does not currently enforce it.
- Source repository has no LICENSE file. No LICENSE file is included, so this archive does not grant third-party reuse rights. The repository owner must state applicable distribution terms separately.

Read `skills/fit-coach/SKILL.md` first. It points to the four canonical reference files and states the runtime boundaries.

