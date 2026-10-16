# MTL-XF-028 — Required deliverables

**Commissioned decision:** Which local-authority and sector combinations warrant decarbonisation programme investigation based on emissions scale, trend and realistic local influence?

All locations below refer to the team's delivery repository. The master repository defines the requirements and contains no completed analysis. Owners are assigned from [the project roles](PROJECT_BRIEF.md).

## D1 — Discovery & decision requirements

**Due:** Week 1  
**Team artefact location:** `docs/01-discovery/`

Decision statement; stakeholder map; as-is reporting to investigation-review process; at least eight prioritised requirements. Answer these questions: Which LA/sector combinations account for the greatest emissions burden? Where are comparable emissions falling slowly or increasing? How does the picture change between territorial and locally influenceable scopes? Are changes driven by sector mix or shifts within sectors? Which additional cost, feasibility and delivery evidence is required for programme investment?

**Acceptance evidence:** All requirements have an owner, priority, deliverable and test ID; domain analyst approves scope.

## D2 — Governed sources & cohort

**Due:** Week 2  
**Team artefact location:** `docs/02-data-governance/; data/`

Freeze the agreed DESNZ 2005–2024 local-authority greenhouse-gas XLSX, approximately 24.9 MB in the prior agreement. Use this workbook rather than the 82.6 MB CSV. Record sheets, units, gases, revisions and territorial/within-influence definitions from actual metadata. Default analysis covers English local authorities; retain other UK areas separately for context. Register exact files, metadata, licences, checksums, coverage and critical fields; record rejection of unavailable dimensions.

**Acceptance evidence:** 100% of inputs registered; no claimed freeze until acquisition evidence exists.

## D3 — Reproducible analytical model

**Due:** Week 3  
**Team artefact location:** `src/; sql/; docs/03-data-model/`

Year × local-authority code × sector/subsector × gas/CO2e basis × territorial or within-influence scope. Keep source totals and subsector details at separate hierarchy levels. Deliver load, type checks, hierarchy handling, lineage, exclusions and environment instructions.

**Acceptance evidence:** A second member regenerates equivalent curated outputs from identical inputs; no unexplained duplicate analytical keys.

## D4 — Quality & reconciliation

**Due:** Week 3  
**Team artefact location:** `docs/04-data-quality/; tests/`

Profile missingness, suppression, valid values, keys and join coverage. Reconcile five LA/year/sector figures and one authority total bridge. Verify tonnes versus kilotonnes conversion with a worked example. Test nonpositive baselines and a boundary-change exclusion. Show shortlist sensitivity to two weight sets and distinguish territorial from influenceable scope.

**Acceptance evidence:** Every input row is accounted for as retained, excluded or quarantined; five published cells reconcile within declared rounding.

## D5 — KPI catalogue

**Due:** Week 4  
**Team artefact location:** `docs/05-kpi-catalogue/`

Define all 8 measures listed below with formula, grain, denominator, unit, source fields, exclusions, owner, refresh and limitations.

**Acceptance evidence:** 100% headline metrics trace to source fields and tested transformations; conditional unavailable measures are explicitly marked.

## D6 — Domain analytical assessment

**Due:** Week 5  
**Team artefact location:** `analysis/; docs/06-analysis/`

Build territorial emissions trend and sector contribution bridges, reconciling totals at declared hierarchy. Compare 2005 baseline and recent five-year patterns; isolate boundary changes and negative/net emission categories.

**Acceptance evidence:** At least five evidence-backed findings state period, population, comparison, magnitude, uncertainty and limitation; negative findings count.

## D7 — Investigation decision framework

**Due:** Week 6  
**Team artefact location:** `docs/07-decision-framework/`

Prioritise up to ten LA/sector investigation cases using burden, trend and a documented local-influence assessment; test at least two weight sets. Record eligibility, thresholds, weights if used, reason codes and manual review triggers.

**Acceptance evidence:** Every shortlisted case has metrics, rationale, owner and evidence gaps; at least two scenarios compared; fewer than ten is valid where evidence is insufficient.

## D8 — BI decision-support product

**Due:** Draft Week 6; final Week 7  
**Team artefact location:** `dashboard/`

Executive overview answering 'Which local-authority and sector combinations warrant decarbonisation programme investigation based on emissions scale, trend and realistic local influence?' plus diagnostic and data-quality views; visible periods, units, denominator notes, resettable filters and accessible labels.

**Acceptance evidence:** Five headline measures reconcile; every filter tested; export screenshots/PDF plus reproducible build or free access instructions.

## D9 — Independent assurance & UAT

**Due:** Week 7  
**Team artefact location:** `docs/08-assurance-uat/`

At least ten scenarios including the four project-specific tests below; requirement-to-test matrix, expected/actual evidence, defect log and simulated stakeholder feedback.

**Acceptance evidence:** No unresolved critical/high defect; accepted lower-severity limitations have a named reviewer and explicit impact.

## D10 — Technical & operational handover

**Due:** Week 8  
**Team artefact location:** `docs/09-technical-handover/`

Clean setup, architecture, frozen input manifest, run/refresh steps, output checks, troubleshooting and change-control process for Local Net Zero Emissions, Sector Decarbonisation & Intervention Prioritisation Intelligence.

**Acceptance evidence:** Another member reproduces the core outputs without undocumented edits and records environment, duration and discrepancies.

## D11 — Executive recommendation

**Due:** Week 8  
**Team artefact location:** `deliverables/`

Maximum two-page briefing and 15–20 minute presentation: commissioned decision, five findings, investigation shortlist, sensitivity, missing evidence, responsibilities and next review.

**Acceptance evidence:** Every quantitative claim links to an artefact/metric; no unsupported causal, policy or operational guarantee.

## D12 — Contribution & delivery record

**Due:** Weekly; final Week 8  
**Team artefact location:** `CONTRIBUTIONS.md; delivery issues/PRs`

Record who delivered and reviewed each MTL-XF-028 work package, including domain, governance, engineering, BI and assurance contributions.

**Acceptance evidence:** Every member links to substantive artefacts and review/presentation evidence; commit count alone is insufficient.

## Required KPI definitions

| Metric | Required definition / calculation |
| --- | --- |
| Emissions | Published emissions in the workbook's stated unit and gas/CO2e scope. |
| Sector share | 100 × compatible sector emissions / matching authority total; avoid double counting subsectors. |
| Change since 2005 | Current minus 2005 emissions, with percentage change only for a valid positive base. |
| Recent five-year change | 2024 minus 2019 emissions, subject to compatible boundaries and actual availability. |
| Per-capita emissions — conditional | Emissions / compatible published population where present; state conversion to tonnes per person. |
| Locally influenceable share — conditional | 100 × within-influence emissions / compatible territorial emissions where both definitions are supported. |
| Reduction contribution | Sector absolute reduction / total authority reduction, with sign and near-zero-total caveats. |
| Coverage | Valid comparable LA/sector/year cells / expected selected cohort cells. |

For every metric record business purpose, formula, source fields, grain, unit, numerator/denominator, exclusions, suppression, zero-base behaviour, owner, refresh and test evidence. Do not populate conditional metrics from invented fields.

## Mandatory domain scenarios

1. Reconcile five LA/year/sector figures and one authority total bridge.
2. Verify tonnes versus kilotonnes conversion with a worked example.
3. Test nonpositive baselines and a boundary-change exclusion.
4. Show shortlist sensitivity to two weight sets and distinguish territorial from influenceable scope.

## Review gates

Week 2: cohort and source approval. Week 4: model, DQ and metrics approval. Week 6: analytical and decision-framework review. Week 8: UAT, independent rerun and final panel review. Record reviewer, date, artefact version and decision at every gate.
