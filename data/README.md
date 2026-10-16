# MTL-XF-028 — Data workspace

## Required sources and cohort

DESNZ local/regional greenhouse-gas data tables, 2005–2024. The Excel workbook is 24.9 MB and is preferable to the 82.6 MB raw CSV for Mettelo.

Freeze the agreed DESNZ 2005–2024 local-authority greenhouse-gas XLSX, approximately 24.9 MB in the prior agreement. Use this workbook rather than the 82.6 MB CSV. Record sheets, units, gases, revisions and territorial/within-influence definitions from actual metadata. Default analysis covers English local authorities; retain other UK areas separately for context.

[Source register and exact URLs](SOURCE_REGISTER.md)

**Current state:** specification only. No raw datasets have been downloaded or uploaded in this build. Expected size, row count and history statements from the earlier agreement require verification against the actual files. Do not mark the cohort frozen until the manifest and metadata are complete.

## Controlled acquisition and preparation

1. Read [SOURCE_REGISTER.md](SOURCE_REGISTER.md); use the exact agreed URLs and official publisher documentation.
2. Validate that the response is the expected CSV/ODS/XLSX/ZIP rather than an error page. Inspect archive contents and sheet names where relevant.
3. Record resolved URL, UTC retrieval, release, coverage, filename, bytes, SHA-256 and licence evidence. Log discrepancies before changing sources.
4. Preserve original bytes in an approved immutable snapshot; later upload only where instructed and redistribution is permitted.
5. Record source fields, types, valid values, suppression, units and publisher methodology in [metadata](metadata/README.md).
6. Implement the analytical grain below, verify keys/cardinality and account for excluded/quarantined records.
7. Reconcile at least five published measures and create curated outputs reproducibly in the team repository.

## Analytical grain

Year × local-authority code × sector/subsector × gas/CO2e basis × territorial or within-influence scope. Keep source totals and subsector details at separate hierarchy levels.

## Required metric contract

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

## Mandatory quality risks

- Territorial emissions and emissions within local influence are different scopes.
- Historical reductions do not prove a local policy caused them; investment recommendations need cost and feasibility evidence.
- Treat negative/net emissions and land-use categories explicitly; no unqualified percentage ranking on nonpositive baselines.

1. Reconcile five LA/year/sector figures and one authority total bridge.
2. Verify tonnes versus kilotonnes conversion with a worked example.
3. Test nonpositive baselines and a boundary-change exclusion.
4. Show shortlist sensitivity to two weight sets and distinguish territorial from influenceable scope.

## Folder ownership

- [raw](raw/README.md): unmodified approved source snapshots; guidance only at present.
- [reference](reference/README.md): governed code lists, hierarchies and crosswalks.
- [metadata](metadata/README.md): source notices, schema, glossary, lineage and manifest evidence.

Curated data, processing code, logs and test results belong in the team delivery repository. Preserve a reproducible boundary between source inputs and generated products. Do not add personal, confidential or paid-source data.
