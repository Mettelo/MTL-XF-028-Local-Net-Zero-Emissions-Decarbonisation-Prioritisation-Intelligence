# MTL-XF-028 — Project brief

This is a **simulated confidential-client engagement using official public/open data**. Client and stakeholder role labels describe a fictional engagement; do not claim a real external Mettelo customer, employment, endorsement or privileged data access. No raw data is uploaded by this specification update.

**Client:** Confidential Combined Authority Net Zero & Programme Investment Board. **Decision owner:** Director of Net Zero & Climate Programme Investment. **Team:** 6–8. **Duration:** 8 weeks. **Review:** annual emissions baseline review and quarterly programme-prioritisation meeting.

## Business problem and commission

The simulated combined-authority net-zero board allocates feasibility and programme-development attention across places and sectors. Its quarterly prioritisation meeting must decide which decarbonisation opportunities deserve further work before any investment proposal is considered.

The Director of Net Zero & Climate Programme Investment needs to move from an emissions inventory to a practical feasibility agenda. A large territorial source may offer little direct local influence, while an area with a smaller but persistent transport or building-related signal may present a more actionable question. Historical reductions can also reflect national electricity changes or industrial activity rather than local programme delivery.

A simple carbon ranking therefore cannot explain where the authority should spend its next tranche of feasibility effort. The commission is a transparent LA/sector opportunity screen combining emissions scale and trend with a separately evidenced local-influence assessment, so programme managers can commission the right cost, delivery and partner enquiries.

> Which local-authority and sector combinations warrant decarbonisation programme investigation based on emissions scale, trend and realistic local influence?

**Required management handover:** A net-zero feasibility screening pack with reconciled sector-change bridges, a distinct local-influence assessment, two weighting scenarios and a programme enquiry register specifying the evidence required before an investment case.

See [the management use case](BUSINESS_CONTEXT.md#practical-management-use-case) for how the review meeting uses this evidence.

## Core deliverable boundary

Agreed DESNZ workbook, 2005–2024. Default screening covers English LA/sector records; recent comparison uses 2019–2024, with 2005 as the long-run reference where a valid positive baseline exists. Use a single inventory revision and boundary basis. Territorial total greenhouse gases remain separate from any narrower local-influence measure. Present at most ten shortlisted LA/sector cases for feasibility investigation.

**Optional / out of core:** Cost per tonne, investment returns, consumption-based emissions, future target delivery and causal local-policy attribution need additional evidence. Confirm the gas scope of within-influence tables before comparing with total GHG; do not assume they share coverage.

File availability does not prove dimensional support. Before analytical build, the team completes the source→field→metric→deliverable matrix in [data guidance](../data/README.md). Missing mandatory support blocks the gate and requires an approved official replacement or scope decision.

## Analytical model

Year × local-authority code × sector/subsector × gas/CO2e basis × territorial or within-influence scope. Keep source totals and subsector details at separate hierarchy levels.

The source contract above controls where a general grain description is conditional. Do not create dimensions absent from the approved input.

## Objectives

1. Every carbon result identifies gas/CO2e scope, mass unit, inventory version and geography.
2. Every priority case has a separate local-influence justification and cost/feasibility evidence request.
3. Both weight sets disclose component values and changes in shortlisted cases.

## Business questions

1. Which LA/sector combinations account for the greatest emissions burden?
2. Where are comparable emissions falling slowly or increasing?
3. How does the picture change between territorial and locally influenceable scopes?
4. Are changes driven by sector mix or shifts within sectors?
5. Which additional cost, feasibility and delivery evidence is required for programme investment?

## Cross-functional delivery model

| Delivery role | Required project contribution |
| --- | --- |
| Business Analyst / Delivery Lead | Map the annual emissions baseline review and quarterly programme-prioritisation meeting, document eight prioritised user requirements and maintain requirement→deliverable→test links; Director of Net Zero & Climate Programme Investment owns business approval. |
| Data Governance Analyst | Own the MTL-XF-028 source/metadata register, cohort decision, licence evidence and 100% headline-measure lineage; resolve the specific risk: Local influence, inventory revisions and gas/unit differences can create misleading decarbonisation priorities. |
| Data Engineer | Implement the declared facts, keys, hierarchy and join controls; account for every source row and deliver a second-member reproducible run at the chosen MTL-XF-028 scope. |
| BI Developer | Implement the annual emissions baseline review and quarterly programme-prioritisation meeting overview, diagnostic and quality pages; reconcile five measures and ensure cohort/extension warnings survive filters and export. |
| Sustainability & Emissions Analyst | Validate gas/unit/scope definitions, five source reconciliations and sector bridges. |
| Net Zero Programme Analyst | Own local-influence assumptions and attach cost/feasibility evidence gaps to each shortlisted case. |
| Climate Decision Assurance Analyst | Review two prioritisation weight sets, boundary treatment and causal-claim limitations. |

Assign named team members and review partners at kickoff; roles may be combined, but a distinct member must review critical calculations and perform the final clean rerun. The executive and operational stakeholder roles are specified in [business context](BUSINESS_CONTEXT.md).

## Required investigation approach

Provide transparent component ranks for current burden, recent reduction trend and documented local influence. Compare a burden-led weight set (60/20/20) with a more balanced set (40/30/30). Define component direction, eligibility and missingness before applying weights; do not score a missing influence assessment as zero. Weights are simulated planning assumptions.

## Milestones and acceptance

| Gate | Reviewers | Evidence / decision |
| --- | --- | --- |
| G1 — scope/source, end Week 2 | Business Analyst + Data Governance Analyst + domain specialist | Approve actual period, geography, grain, required input and field support in a source-to-deliverable matrix. Workbook listing, revision/boundary context and scope distinction verified; sheet-level mappings, precise gas/unit compatibility and frozen checksums pending. Unsupported mandatory outputs remain blocked, not quietly reclassified as completed. |
| G2 — model/metrics, end Week 4 | Data Engineer + domain specialist + independent reviewer | Approve row accounting, keys, hierarchy, join cardinality, five source reconciliations and all core metric definitions. |
| G3 — analytical decision review, end Week 6 | Director of Net Zero & Climate Programme Investment + operational stakeholders | Provide transparent component ranks for current burden, recent reduction trend and documented local influence. Compare a burden-led weight set (60/20/20) with a more balanced set (40/30/30). Define component direction, eligibility and missingness before applying weights; do not score a missing influence assessment as zero. Weights are simulated planning assumptions. Retain an evidence-insufficient case and a manual review route. |
| G4 — release, end Week 8 | Simulated Mettelo panel + independent reviewer | Accept D1–D12 only after ten executed domain tests, five BI reconciliations, clean rerun evidence and resolution of all critical/high defects. |

D1–D12 are defined in [deliverables](DELIVERABLES.md). AC1–AC12 and DT1–DT10 are defined in [acceptance criteria](ACCEPTANCE_CRITERIA.md). No real production deployment, automatic funding/service allocation, private-client data or paid-source dependency is required.
