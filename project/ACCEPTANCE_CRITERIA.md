# MTL-XF-028 — Acceptance criteria and domain tests

**Business decision owner:** Director of Net Zero & Climate Programme Investment. **Decision:** Which local-authority and sector combinations warrant decarbonisation programme investigation based on emissions scale, trend and realistic local influence?

## Delivery sign-off

| ID | Deliverables | Required pass evidence | Acceptance owner |
| --- | --- | --- | --- |
| AC1 | D1 | Eight user requirements cover the commissioned questions, named stakeholder actions and core/extension boundary. | Business Analyst / Director of Net Zero & Climate Programme Investment |
| AC2 | D2 | 100% of used source files have approved provenance, version/coverage, licence, retrieval UTC and SHA-256. Required fields and reference versions are checked. | Data Governance Analyst |
| AC3 | D3 | Every input row is accounted for; keys and all many-to-many/hierarchy effects have explicit checks and no unexplained duplication. | Data Engineer / independent reviewer |
| AC4 | D4 | Five source cells reconcile within a declared rounding tolerance; all material differences and non-additive totals are explained. | Domain specialist |
| AC5 | D5 | All 8 metric contracts are classified core/conditional and have tested definitions; no unsupported fields or fabricated unavailable values. | Data Governance Analyst / BI Developer |
| AC6 | D6 | Five findings cover all business questions or evidence gaps; period, eligible population, magnitude, comparison and limitation are visible. | Domain analyst |
| AC7 | D7 | The project-specific baseline and alternative below are implemented; eligibility, scenario changes, reason codes and evidence requests are visible. | Director of Net Zero & Climate Programme Investment |
| AC8 | D8 | Five BI measures reconcile to curated outputs; all filters/reset/export retain the scope, units and limitations. | BI Developer / operational UAT user |
| AC9 | D9 | DT1–DT10 have actual execution evidence and expected/actual outcomes; no unresolved critical/high defect. | Independent reviewer |
| AC10 | D10 | A distinct member's clean rerun reproduces equivalent core outputs with documented environment and checks. | Independent rerun reviewer |
| AC11 | D11 | Two-page maximum briefing and 15–20 minute presentation answer the decision and assign investigation owners without unsupported outcomes. | Director of Net Zero & Climate Programme Investment / Mettelo panel |
| AC12 | D12 | Every member links substantive authored and reviewed work, including handover or presentation contribution. | Delivery Lead |

## Project-specific business success

1. Every carbon result identifies gas/CO2e scope, mass unit, inventory version and geography.
2. Every priority case has a separate local-influence justification and cost/feasibility evidence request.
3. Both weight sets disclose component values and changes in shortlisted cases.

## Required prioritisation and sensitivity

Provide transparent component ranks for current burden, recent reduction trend and documented local influence. Compare a burden-led weight set (60/20/20) with a more balanced set (40/30/30). Define component direction, eligibility and missingness before applying weights; do not score a missing influence assessment as zero. Weights are simulated planning assumptions.

Record each case's entity/segment, valid period, supporting measures, reason code, scenario position, missing evidence, responsible operational role, next review and manual-review trigger. Fewer than ten cases is valid; padding unsupported cases fails acceptance.

## DT1–DT10 — minimum executed domain tests

| Test | Input / action | Expected pass evidence |
| --- | --- | --- |
| DT1 | Reconcile five LA/year/sector figures and one authority total bridge. | Five selected published values reproduce within declared source precision, with explicit source coordinates and scope. |
| DT2 | Verify tonnes versus kilotonnes conversion with a worked example. | The invalid comparison, join or denominator is rejected or flagged according to the documented rule; no silent fallback. |
| DT3 | Test nonpositive baselines and a boundary-change exclusion. | The edge case produces an explicit unavailable/exclusion result or a supported calculation, with affected rows quantified. |
| DT4 | Show shortlist sensitivity to two weight sets and distinguish territorial from influenceable scope. | The domain boundary remains visible in the analytical output and BI product; no unsupported inference. |
| DT5 | 1 kilotonne CO2e is converted for a per-person measure | Equals 1,000 tonnes CO2e; denominator and resulting unit remain explicit. |
| DT6 | A total-GHG territorial value is compared with a CO2-only influence table | Do not report the ratio as a like-for-like influenceable GHG share. |
| DT7 | Baseline emissions are negative or zero | Percentage reduction is unavailable; retain absolute change with explanation. |
| DT8 | Data from two inventory revisions is mixed | Reject or reconcile the mixture before calculating trends. |
| DT9 | Weights change from 60/20/20 to 40/30/30 | Scores and shortlist membership are recomputed with unchanged eligibility. |
| DT10 | Local influence is unknown | Mark evidence missing and hold the case for review rather than assign a fabricated score. |

Worked values are **synthetic test fixtures**, not claims about the public data or simulated client. For each test retain requirement ID, source/input or fixture, expected result, actual result, evidence link, tester, independent reviewer and date. DT1–DT4 additionally require the documented project-specific rule; their general evidence descriptions do not waive the named domain condition. Add dashboard/filter tests as needed beyond these ten.

## Scope gate and unresolved issues

**Mandatory core:** Agreed DESNZ workbook, 2005–2024. Default screening covers English LA/sector records; recent comparison uses 2019–2024, with 2005 as the long-run reference where a valid positive baseline exists. Use a single inventory revision and boundary basis. Territorial total greenhouse gases remain separate from any narrower local-influence measure. Present at most ten shortlisted LA/sector cases for feasibility investigation.

**Optional extensions:** Cost per tonne, investment returns, consumption-based emissions, future target delivery and causal local-policy attribution need additional evidence. Confirm the gas scope of within-influence tables before comparing with total GHG; do not assume they share coverage.

A mandatory source/field gap blocks the affected deliverable and must be resolved by a registered official replacement or approved, versioned scope change. An explicitly optional result may be unavailable with a reason and a useful evidence request. Neither missing raw data nor unexecuted tests may be marked passed.

A critical/high defect materially changes a headline value, cohort, recommendation, provenance or reproducibility and blocks release. Lower-impact issues require a named acceptance owner and disclosed impact. All panel feedback and approvals must be recorded honestly as simulated where applicable.
