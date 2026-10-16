# MTL-XF-028 — Local Net Zero Emissions, Sector Decarbonisation & Intervention Prioritisation Intelligence

**Mettelo Project Studio** · Cross-Functional · Master project specification  
**Client:** Confidential Combined Authority Net Zero & Programme Investment Board  
**Accountable simulated executive:** Director of Net Zero & Climate Programme Investment  
**Sector:** Climate / Local Government / Sustainability  
**Team:** 6–8 people · **Window:** 8 weeks  
**Status:** documentation revised; file acquisition and cohort freeze pending  
**Review cadence:** annual emissions baseline review and quarterly programme-prioritisation meeting

> This is a **simulated confidential-client engagement using official public/open data**. Client and stakeholder role labels describe a fictional engagement; do not claim a real external Mettelo customer, employment, endorsement or privileged data access. No raw data is uploaded by this specification update.

## Business problem

The combined authority must choose which sector/place opportunities deserve feasibility work, but the largest territorial emission source may lie outside its direct influence. Changes caused by national electricity supply or industrial activity can also dominate a local trend without demonstrating local policy success. A defensible investment discussion needs a consistent inventory and a separate assessment of delivery influence.

## Commissioned decision

> Which local-authority and sector combinations warrant decarbonisation programme investigation based on emissions scale, trend and realistic local influence?

## Practical use

The Director compares a high-emissions LA/transport combination with an area whose emissions are falling slowly. The team opens the sector bridge, checks whether the change is structural, and records whether local programme levers are plausible. The shortlist commissions feasibility and cost work; it does not approve investment solely from a carbon ranking.

The full [business context](project/BUSINESS_CONTEXT.md) names operational stakeholders, decisions, risks and proposed benefit measures.

## What must be delivered

1. Build territorial emissions trend and sector contribution bridges, reconciling totals at declared hierarchy.
2. Compare 2005 baseline and recent five-year patterns; isolate boundary changes and negative/net emission categories.
3. Prioritise up to ten LA/sector investigation cases using burden, trend and a documented local-influence assessment; test at least two weight sets.

The complete D1–D12 pack includes discovery, source governance, ingestion/model, quality, metric catalogue, analysis, investigation scenarios, BI, assurance/UAT, independent handover, executive briefing and contribution evidence. A dashboard by itself does not satisfy the commission.

## Fixed core and optional work

**Core:** Agreed DESNZ workbook, 2005–2024. Default screening covers English LA/sector records; recent comparison uses 2019–2024, with 2005 as the long-run reference where a valid positive baseline exists. Use a single inventory revision and boundary basis. Territorial total greenhouse gases remain separate from any narrower local-influence measure. Present at most ten shortlisted LA/sector cases for feasibility investigation.

**Extensions:** Cost per tonne, investment returns, consumption-based emissions, future target delivery and causal local-policy attribution need additional evidence. Confirm the gas scope of within-influence tables before comparing with total GHG; do not assume they share coverage.

Source support is checked at the Week 2 gate. A required output is blocked until its fields and cohort are verified; it cannot pass acceptance through a generic “data unavailable” disclaimer. An explicitly optional extension may remain unavailable with a reason. See [exact source URLs and verification evidence](data/SOURCE_REGISTER.md).

## Measurable project outcomes

1. Every carbon result identifies gas/CO2e scope, mass unit, inventory version and geography.
2. Every priority case has a separate local-influence justification and cost/feasibility evidence request.
3. Both weight sets disclose component values and changes in shortlisted cases.

All headline metrics require field lineage; five source values and five BI measures must reconcile. DT1–DT10 must be executed, a second member must reproduce the core outputs, and no critical/high defect may remain. These assess delivery quality; real-world savings or service improvement are not claimed.

## Investigation rules

Provide transparent component ranks for current burden, recent reduction trend and documented local influence. Compare a burden-led weight set (60/20/20) with a more balanced set (40/30/30). Define component direction, eligibility and missingness before applying weights; do not score a missing influence assessment as zero. Weights are simulated planning assumptions.

- Territorial emissions and emissions within local influence are different scopes.
- Historical reductions do not prove a local policy caused them; investment recommendations need cost and feasibility evidence.
- Treat negative/net emissions and land-use categories explicitly; no unqualified percentage ranking on nonpositive baselines.

## Team and stakeholder ownership

Director of Net Zero & Climate Programme Investment approves business scope and the investigation recommendation. The Business Analyst, Data Governance Analyst, Data Engineer and BI Developer work with the specialist roles in the [project brief](project/PROJECT_BRIEF.md). Assign individual owners at kickoff and record substantive work and independent reviews in `CONTRIBUTIONS.md`.

## Delivery plan

Weeks 1–2: decision requirements and verified cohort. Weeks 3–4: model, reconciliation and metric definitions. Weeks 5–6: analytical findings, alternative investigation scenarios and BI draft. Weeks 7–8: simulated UAT, independent rerun, executive briefing and handover.

## Start here

1. [Project brief](project/PROJECT_BRIEF.md) and [business context](project/BUSINESS_CONTEXT.md).
2. [D1–D12 deliverables and metric contracts](project/DELIVERABLES.md).
3. [AC1–AC12 and DT1–DT10 acceptance tests](project/ACCEPTANCE_CRITERIA.md).
4. [Governance and sign-off](project/GOVERNANCE.md).
5. [Data workspace](data/README.md), [source register](data/SOURCE_REGISTER.md), [raw](data/raw/README.md), [reference](data/reference/README.md) and [metadata](data/metadata/README.md) guidance.
6. [Team repository standard](submission/TEAM_REPOSITORY_STANDARD.md), [submission guide](submission/SUBMISSION_GUIDE.md) and [final template](submission/FINAL_SUBMISSION_TEMPLATE.md).

## Master and team repositories

This master repository holds the Mettelo-controlled specification. Create `MTL-XF-028-<team-name>` under the **Mettelo GitHub organisation** and add every member's individual account. Delivery analysis, code, tests, BI and contribution evidence belong in that team repository. Use issues, branches, meaningful commits, PRs and reviews where practical.

The required master areas are `project/`, `data/` (including raw/reference/metadata guidance) and `submission/`; [the documentation index](project/README.md) explains their authority and current revision.

**Mettelo — Built for What’s Next**
