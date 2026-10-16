# MTL-XF-028 — Data workspace and support gate

## Core contract

Agreed DESNZ workbook, 2005–2024. Default screening covers English LA/sector records; recent comparison uses 2019–2024, with 2005 as the long-run reference where a valid positive baseline exists. Use a single inventory revision and boundary basis. Territorial total greenhouse gases remain separate from any narrower local-influence measure. Present at most ten shortlisted LA/sector cases for feasibility investigation.

## Optional work

Cost per tonne, investment returns, consumption-based emissions, future target delivery and causal local-policy attribution need additional evidence. Confirm the gas scope of within-influence tables before comparing with total GHG; do not assume they share coverage.

## Acquisition state

No raw data is uploaded by this update. Official documentation checks are recorded in [SOURCE_REGISTER.md](SOURCE_REGISTER.md). File payloads, full schemas, bytes/checksums and final reuse/freeze approvals remain pending where stated. Keep publication-level evidence distinct from acquired-file evidence.

## Required source-to-deliverable matrix

Before analysis, create a row per headline measure/required comparison:

`requirement_id | deliverable_id | metric | core_or_extension | source_id | actual_field_or_sheet | valid_grain | coverage | unit_denominator | metadata_evidence | support_status | owner | decision`

Allowed support statuses: documentation-supported; payload-verified; unsupported; optional-not-activated. “Documentation-supported” alone is insufficient for a completed data freeze. If a mandatory field is absent, block its output and resolve the source or approved scope; do not fabricate values or silently waive the requirement.

## Controlled preparation

1. Use registered exact URLs and inspect actual content type, archive members or sheets.
2. Record version, resolved URL, separate retrieval timestamps, bytes, SHA-256 and licence evidence.
3. Approve the actual cohort and scope matrix at G1.
4. Preserve original bytes; transform into curated facts with documented types, keys, hierarchies and joins.
5. Account for retained/excluded/quarantined rows and quantify all mapping gaps.
6. Reconcile five source values and execute [DT1–DT10](../project/ACCEPTANCE_CRITERIA.md).

## Model and measures

Year × local-authority code × sector/subsector × gas/CO2e basis × territorial or within-influence scope. Keep source totals and subsector details at separate hierarchy levels.

The core contract above controls conditional dimensions. Metric formulas have one authoritative home: [DELIVERABLES.md](../project/DELIVERABLES.md). Do not create another incompatible formula copy in the data README.

## Data areas

- [Raw snapshots](raw/README.md): unmodified source bytes only when later authorised and permitted.
- [Reference data](reference/README.md): category/entity/period mappings with version and cardinality.
- [Metadata](metadata/README.md): manifest, dictionary, methodology, lineage and support/freeze decisions.

**Specific control:** Local influence, inventory revisions and gas/unit differences can create misleading decarbonisation priorities.
