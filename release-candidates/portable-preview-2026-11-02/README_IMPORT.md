# Fit_Coach SID — portable import package (review preview)

**Build date:** 2026-11-02  
**Source:** Fit_Coach_Plugin PR #1 head `b6970cebff3c17fbad32a66a51ae8ac9ae8aa7ed`; canonical fitness files are copied unchanged from source commit `06f7558b327068c414d252528741d0918e141cbc`.  
**Status:** Import-format preparation only. Expert/domain approval, product benchmark, user pilot, and successful installation on each live host are **NOT RUN**. This archive is not a validated coaching release.

This is one downloadable archive containing host-specific setup material. GPT, Claude and Gemini do **not** share one native plugin installer. Use the adapter for the host you choose:

## ChatGPT / a Custom GPT

1. Open `gpt/Instructions.md` and copy it into the GPT's **Instructions** field.
2. Upload the four files in `gpt/knowledge/` as separate knowledge files. Knowledge files provide reference material; instructions define behavior.
3. If the GPT is for coaching, keep `case-benchmark.md` marked as evaluation-only in the instructions. Do not treat it as scientific evidence.
4. Test with the platform's preview before relying on the result. A successful upload is not product/domain validation.

**Availability note (checked 2026-11-02):** OpenAI's help currently says new custom GPT creation/publication is unavailable on personal ChatGPT accounts and that existing GPT editing depends on eligibility/permissions; a staged migration to plugins is underway. Enterprise/workspace and migration availability can differ. If GPT creation/editing is unavailable to your account, keep this package as the source bundle for the applicable migrated skill/plugin workflow. See [OpenAI GPT creation/editing](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts) and [migration FAQ](https://help.openai.com/en/articles/20001519-custom-gpt-retirement-and-migration-faq).

## Claude

Upload `claude/fit-coach-sid-skill.zip` through **Customize → Skills → Create skill → Upload a skill**. The ZIP contains one `fit-coach-sid/` folder with `SKILL.md` and its `references/`. Skill availability depends on plan, account settings and organization policy. See [Claude: use Skills](https://support.claude.com/en/articles/12512180-use-skills-in-claude) and [create custom Skills](https://support.claude.com/en/articles/12512198-how-to-create-custom-skills).

## Gemini

For personal accounts where **Skills** is available, upload `gemini/fit-coach-sid-skill.zip` from Gemini's **Customize → Skills** flow. It contains a folder named `fit-coach-sid/`, root `SKILL.md`, and reference files. In the transition period, if only **Gems** is available, create a Gem, paste `gpt/Instructions.md` into its instructions, and upload the four `gpt/knowledge/` files as Knowledge. Work/school rollout and UI availability may differ. See [Gemini Skills upload requirements](https://support.google.com/gemini/answer/17094296) and [Gems-to-Skills transition](https://support.google.com/gemini/answer/18560919).

## Important scope and limits

- This is a portable instruction/reference package, **not** an executable API plugin, medical device, or guarantee that one ZIP installs identically everywhere.
- The portable `SKILL.md`/GPT instructions add an explicit rule: Vietnamese identity informs language and local context only; it must not be used to infer an individual's physiology or dose.
- The four canonical fitness references are included; their domain claims have not received the required independent expert approval. Use imported numeric claims as unverified.
- The benchmark reference is for evaluation only, not a source of coaching truth. No model outputs were generated for this package.
- No LICENSE is included. This ZIP does not grant third-party reuse rights. The repository owner must set distribution terms.
- No fitness-domain, medical, nutrition, or Vietnamese-language review is implied by packaging or upload success.
