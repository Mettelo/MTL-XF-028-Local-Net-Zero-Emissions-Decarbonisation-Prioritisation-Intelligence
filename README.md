# MTL-XF-028 — Local Net Zero Emissions, Sector Decarbonisation & Intervention Prioritisation Intelligence

**Mettelo Project Studio** · Cross-Functional · Master specification  
**Client:** Confidential Combined Authority Net Zero & Programme Investment Board  
**Sector:** Climate / Local Government / Sustainability  
**Status:** Pre-launch; documentation ready, data acquisition/freeze pending  
**Recommended team:** 6–8 people · **Delivery window:** 8 weeks  
**Master repository:** `Mettelo/MTL-XF-028-Local-Net-Zero-Emissions-Decarbonisation-Prioritisation-Intelligence`

> This is a **simulated confidential-client engagement** using official public/open data. The client label is fictional and intentionally anonymous. Do not imply a real external Mettelo customer, employment by that client, privileged access or confidential source data. Public source statistics remain public; the engagement framing does not make them confidential.

## Business challenge

**Local Net Zero Emissions, Sector Decarbonisation & Intervention Prioritisation Intelligence.** A combined authority needs to know which sectors and local authorities contribute most to emissions, where emissions are declining slowly, and where local policy intervention may have the strongest case.

Current reporting fragments the evidence needed for a repeatable management review. The team must explain which signals are reliable, which comparisons are valid and where further investigation is needed. No budget, operational failure or improvement outcome is asserted as an observed client fact.

## Commissioned decision

> Which local-authority and sector combinations warrant decarbonisation programme investigation based on emissions scale, trend and realistic local influence?

The product supports a simulated stakeholder review. A dashboard alone is insufficient: the recommendation must be traceable to governed definitions, a reproducible model, reconciled analysis and a transparent investigation framework.

## Business questions

- Which LA/sector combinations account for the greatest emissions burden?
- Where are comparable emissions falling slowly or increasing?
- How does the picture change between territorial and locally influenceable scopes?
- Are changes driven by sector mix or shifts within sectors?
- Which additional cost, feasibility and delivery evidence is required for programme investment?

## Approved data and cohort

DESNZ local/regional greenhouse-gas data tables, 2005–2024. The Excel workbook is 24.9 MB and is preferable to the 82.6 MB raw CSV for Mettelo.

Freeze the agreed DESNZ 2005–2024 local-authority greenhouse-gas XLSX, approximately 24.9 MB in the prior agreement. Use this workbook rather than the 82.6 MB CSV. Record sheets, units, gases, revisions and territorial/within-influence definitions from actual metadata. Default analysis covers English local authorities; retain other UK areas separately for context.

Exact copyable URLs and acquisition gates are in [SOURCE_REGISTER.md](data/SOURCE_REGISTER.md). No raw data is uploaded by this build. Source coverage and size statements inherited from the agreement are expected values until controlled acquisition verifies them; current URLs are not a substitute for a frozen file manifest.

## What the team must build

1. Build territorial emissions trend and sector contribution bridges, reconciling totals at declared hierarchy.
2. Compare 2005 baseline and recent five-year patterns; isolate boundary changes and negative/net emission categories.
3. Prioritise up to ten LA/sector investigation cases using burden, trend and a documented local-influence assessment; test at least two weight sets.

Produce the full D1–D12 delivery pack: discovery, governance, ingestion/model, quality, KPI catalogue, analysis, decision framework, BI, assurance/UAT, handover, executive briefing and contribution record. [Deliverables](project/DELIVERABLES.md) defines locations, dates and evidence for each.

## Core measures

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

## Cross-functional ownership

| Accountable role | Project responsibility and evidence |
| --- | --- |
| Business Analyst / Delivery Lead | Own the commissioned decision for Confidential Combined Authority Net Zero & Programme Investment Board; record at least eight prioritised requirements, each linked to a deliverable and test; maintain weekly scope and decision logs. |
| Data Governance Analyst | Register every 028 input and critical field; approve the frozen cohort, licence evidence, glossary and 100% headline-KPI lineage before analysis. |
| Data Engineer | Implement the stated 028 analytical grain, ingestion and exclusions; deliver a clean rerun with row-count/checksum evidence and no unexplained key duplicates. |
| BI Developer | Build executive, diagnostic and quality views for the commissioned decision; reconcile at least five 028 dashboard measures and test every visible filter. |
| Sustainability & Emissions Analyst | Validate gas/unit/scope definitions, five source reconciliations and sector bridges. |
| Net Zero Programme Analyst | Own local-influence assumptions and attach cost/feasibility evidence gaps to each shortlisted case. |
| Climate Decision Assurance Analyst | Review two prioritisation weight sets, boundary treatment and causal-claim limitations. |

Roles may be combined by a smaller team, but each responsibility needs a named owner. A different member reviews critical calculations and final evidence wherever practical.

## Interpretation rules

- Territorial emissions and emissions within local influence are different scopes.
- Historical reductions do not prove a local policy caused them; investment recommendations need cost and feasibility evidence.
- Treat negative/net emissions and land-use categories explicitly; no unqualified percentage ranking on nonpositive baselines.

## Measurable success

- All source files and transformations have provenance and licence evidence; approved inputs have SHA-256 manifests.
- All headline metrics have tested definitions and source-field lineage.
- At least five published values and five dashboard measures reconcile with declared source rounding.
- At least five findings address the business questions and quantify materiality.
- Up to ten investigation cases have evidence, reason codes, owners and limitations; at least two priority scenarios are compared.
- At least ten UAT scenarios pass or have explicitly accepted low-impact limitations; no critical/high defect remains.
- A second member reproduces the core outputs from the same frozen inputs.

These are delivery acceptance thresholds, not promises of real-world service improvement. See [acceptance criteria](project/ACCEPTANCE_CRITERIA.md).

## Delivery sequence

Weeks 1–2: decision requirements, source inspection and freeze approval. Weeks 3–4: model, reconciliation and KPI definitions. Weeks 5–6: analysis, investigation framework and BI draft. Weeks 7–8: UAT, independent rerun, briefing and handover.

## Start here

1. Read the [project brief](project/PROJECT_BRIEF.md) and [business context](project/BUSINESS_CONTEXT.md).
2. Review [deliverables](project/DELIVERABLES.md), [acceptance criteria](project/ACCEPTANCE_CRITERIA.md) and [governance](project/GOVERNANCE.md).
3. Inspect the [data workspace](data/README.md), [source register](data/SOURCE_REGISTER.md), [raw guidance](data/raw/README.md), [reference guidance](data/reference/README.md) and [metadata guidance](data/metadata/README.md).
4. Create `MTL-XF-028-<team-name>` under the **Mettelo GitHub organisation**, add each member's individual account and follow the [team repository standard](submission/TEAM_REPOSITORY_STANDARD.md).
5. Use the [submission guide](submission/SUBMISSION_GUIDE.md) and [final submission template](submission/FINAL_SUBMISSION_TEMPLATE.md).

## Master and team repositories

This master holds the challenge specification. Teams deliver their analysis and artefacts in their own Mettelo organisation repository. Do not submit team work by replacing this master specification. Use issues, branches, meaningful commits, PRs and reviews to demonstrate actual collaboration.

## Specification map

```text
README.md
project/README.md
project/PROJECT_BRIEF.md
project/BUSINESS_CONTEXT.md
project/DELIVERABLES.md
project/ACCEPTANCE_CRITERIA.md
project/GOVERNANCE.md
data/README.md
data/SOURCE_REGISTER.md
data/raw/README.md
data/reference/README.md
data/metadata/README.md
submission/README.md
submission/TEAM_REPOSITORY_STANDARD.md
submission/SUBMISSION_GUIDE.md
submission/FINAL_SUBMISSION_TEMPLATE.md
```

**Mettelo — Built for What’s Next**
