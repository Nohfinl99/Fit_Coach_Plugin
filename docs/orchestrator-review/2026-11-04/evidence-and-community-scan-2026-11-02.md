# Fit_Coach evidence and gym-community scan

**Date:** 2026-11-02  
**Scope:** Read-only; supports FC-01/FC-02 planning. No product edits, benchmark run, or GitHub write.  
**Product source:** exact Git commit `06f7558b327068c414d252528741d0918e141cbc`; see [source baseline manifest](source-baseline-2026-11-02.json).

## Findings from gym communities

### Curated international communities

TheFitness.Wiki identifies itself as the wiki for r/Fitness and r/weightroom, curated from threads and community advice. Its FAQ index repeatedly covers practical questions such as choosing a routine, stalled progress, bulking/cutting, motivation, judging a routine, soreness, returning after a break, training splits, rep ranges, training to failure, alternatives, and food choices. These are useful **candidate user-intent categories** for Fit_Coach discovery and tests. The FAQ is not a probability sample, and its topic ordering cannot be treated as the prevalence of user needs.

Stronger by Science's guide index groups resources on goal setting/behavior change and strength training across beginner-to-advanced levels, and links to reviews/studies. It is a practitioner-facing resource. Only the index was inspected for this scan; individual guides and their citations were not audited here.

### Vietnamese community leads

A preliminary search surfaced a long-running VOZ Strength Club thread and public r/VietNam discussions about gym access, prices, equipment, etiquette, and coaching. The inspected material was limited to search snippets, not a sample with a defined recruitment method. Some posts are written by visitors or expatriates and may describe a particular city, gym, time, or one user's experience.

**Finding:** this scan did not verify a large, representative report of Vietnamese gym users' training needs or outcomes. Do not generalize these posts to Vietnamese users as a population. Use them only to form hypotheses for future interviews or usability work, and label them anecdotal. No social-media scraping or reuse of private group data is proposed.

## Evidence sources and applicability

| Source | What it can support | Read depth / limit |
|---|---|---|
| ACSM 2026 resistance-training overview | Broad resistance-training evidence for healthy adults; overview covers 137 systematic reviews and more than 30,000 participants. It supports multiple workable training approaches and emphasizes effort, participation, and individualization. | Full article and relevant results/discussion inspected. Search cutoff was Oct 2024; it is not a clinical screening rule or proof of a specific plan for a Vietnamese person. |
| IUSCA 2021 hypertrophy position stand | Expert synthesis for hypertrophy-focused athletic populations. | Metadata/abstract inspected; not a universal rulebook for recreational beginners. Full paper remains to be read claim-by-claim before use. |
| WHO/MOH Viet Nam STEPS 2021 | Population-level health-risk and anthropometric context in Viet Nam. | WHO report landing page inspected; full report not audited in this pass. It does not test a resistance-training dose or establish a single Vietnamese body type. |
| ISSN protein position stand (2017) | General sports-nutrition education for exercising populations, subject to scope and freshness review. | Abstract/key-point summary inspected. Excluded from individualized numeric prescriptions in V1. |
| Havers et al. (2025) | Expert ratings and reproducibility of AI-generated hypertrophy plans. Eight plans were rated by 12 coaches; richer prompts improved ratings. | Article abstract/design/results summary inspected. This evaluates generated-plan quality, not training outcomes in people. |
| MoveBench (2026) | Rubric-based LLM evaluation across plan generation, sports-data analysis, and Q&A. | Preprint, 809 questions/5,012 rubric criteria. It is an output benchmark, not real-world efficacy; judge reliability and preprint status remain caveats. |
| Exercise/health coaching scoping review (2025) | Map of heterogeneous evaluation designs and gaps across LLM exercise/health coaching studies. | Abstract and selected tables/summary inspected; individual studies not all re-audited. |
| AI exercise interventions in people | Shows that real-user pilots exist, including a 5-week calisthenics intervention with 87 untrained college students. | Secondary review table inspected. Narrow sample/intervention; not evidence for Fit_Coach hypertrophy coaching or Vietnamese users. |

## Current Fit_Coach claim risks

The current `fitness-protocols.md` has a useful source-status gate and an evidence overlay, but the inherited corpus still contains exact defaults whose own rows are `IMPORTED_UNVERIFIED`. Its overlay explicitly says not to use fixed MV/MEV/MAV/MRV bands, mandatory frequency, universal RIR, fixed deload timing, or unregistered rest intervals as approved individualized rules. Examples in the imported rows include fixed set-volume bands, a claimed 8–10-set MEV, 12–20-set MAV, 20–25+ MRV, a hard per-session volume cap, and exact RIR defaults. The ontology also retains absolute or tightly numeric physiological claims.

The current EX-11 row records the 2026 ACSM healthy-adult overview: the review supports a dose-response signal for higher weekly hypertrophy volume (≥10 sets/week), but warns against turning that population-level threshold into a universal individual minimum. For frequency, its broad participation recommendation should not be converted into a claim that every person needs one exact weekly split. The ACSM article reports insufficient data to determine the hypertrophy effect of inter-set rest; any claim that one fixed rest interval guarantees more growth needs a separate, directly applicable source.

Do not resolve these tensions by deleting old text or changing old evidence status in place. Keep the exact claim, source row, status, conflict, and use restriction in a revisioned claim ledger. For V1, omit claims that do not pass the current source gate.

## Claim/applicability ledger for the rebuild

| ID | Claim area | Current evidence status | Allowed use in V1 | Needed next |
|---|---|---|---|---|
| FC-EV-01 | General RT benefits and flexible training forms | EX-11 `APPROVED` within its healthy-adult scope; human domain review still needed | Explain population-level evidence; no promise of individual outcome | Claim-by-claim applicability review, especially age/health boundaries |
| FC-EV-02 | ≥10 weekly sets and hypertrophy | EX-11 `APPROVED` as a population dose-response signal, not an individual minimum | Discuss as one evidence signal; a plan may use a lower starting dose if justified by experience/constraints and label assumptions | Coaches review exact wording and how to count direct/indirect sets |
| FC-EV-03 | MEV/MAV/MRV and fixed volume bands | Imported defaults `IMPORTED_UNVERIFIED` | Do not emit as validated thresholds or individualized numeric rules | Source audit or remove from future candidate with recorded diff |
| FC-EV-04 | Universal RIR/failure prescription | EX-04/10/11 cover bounded claims; exact universal defaults remain unverified | Explain that failure is not mandatory; effort targets require qualified source/context and calibration | Define when effort scales are useful and test novice estimation limits |
| FC-EV-05 | Rest interval and hypertrophy | Current ACSM overview reports insufficient evidence to determine the effect | Give practical rest guidance only as an effort/recovery/feasibility choice if supported; do not claim a guaranteed hypertrophy advantage from a fixed interval | Reconcile ontology and protocol wording against primary sources |
| FC-EV-06 | Deload schedule, fixed session cap, CNS/tendon/immune claims | Imported defaults `IMPORTED_UNVERIFIED` unless a specific approved row is found | Do not prescribe a fixed deload calendar or diagnose CNS/immune/tendon state | Audit each claim and map objective monitoring signals |
| FC-EV-07 | Vietnamese population/body type | Population data are not a single-person phenotype or training-dose source | Use language, units, food/equipment availability, and user-provided measurements/logs; keep unsupported response differences `UNKNOWN` | Review full Viet Nam STEPS report; identify Vietnamese intervention research without requiring it to validate all general guidance |
| FC-EV-08 | Nutrition/supplements | Legacy protocol rows include many precise numeric claims; current scope/source review is incomplete | V1 gives general education and local food substitutions without individualized calorie/macro/supplement doses | Separate nutrition claim audit before expanding product scope |
| FC-EV-09 | Competition / rapid cutting / peak week | High-risk area, excluded from V1; SAFE-03 boundary applies | No water/sodium depletion, diuretic, heat or rapid-cut protocols | Keep only safety boundary regression cases |

## Vietnamese-context interpretation

The user's stated Vietnamese context is remembered as a **localization constraint**. No personal height, weight, waist, age, training history, health screen, or training log is supplied in this task, so this report does not infer his body composition, strength potential, recovery, metabolism, or appropriate workload.

For product behavior, use kg/cm and Vietnamese language; offer familiar food/equipment substitutions only when relevant; ask for the individual's measurements/preferences when needed; and test stereotyping explicitly. Population-specific screening references, if later included, must be labelled as screening context and must not alter hypertrophy volume, effort, or progression without individual evidence.

## Source links

- [ACSM 2026 position stand](https://pmc.ncbi.nlm.nih.gov/articles/PMC12965823/)
- [IUSCA 2021 hypertrophy position stand](https://journal.iusca.org/index.php/Journal/article/view/81)
- [WHO/MOH Viet Nam STEPS 2021](https://www.who.int/publications/i/item/9789290620266)
- [TheFitness.Wiki](https://thefitness.wiki/) and [community FAQ](https://thefitness.wiki/faq/)
- [Stronger by Science guides](https://www.strongerbyscience.com/guides/)
- [Havers et al. 2025](https://www.termedia.pl/Reproducibility-and-quality-of-hypertrophy-related-training-plans-generated-by-GPT-4-and-Google-Gemini-as-evaluated-by-coaching-experts%2C78%2C55336%2C0%2C1.html)
- [MoveBench preprint](https://arxiv.org/abs/2610.26185)
- [Scoping review on evaluation strategies](https://pmc.ncbi.nlm.nih.gov/articles/PMC12520646/)
- [Systematic review of exercise/training prescription AI](https://www.mdpi.com/2076-3417/15/7/3497)
- Vietnamese community leads: [VOZ Strength Club](https://voz.vn/t/voz-strength-club-tap-huong-dan-thao-luan-giao-luu-ver-2024.972189/) and a [public r/VietNam thread](https://www.reddit.com/r/VietNam/comments/1h6t50e/whats_your_biggest_challenge_with_staying_fit_in/) (anecdotal search leads only).
