# MTL-XF-028 — Metadata, lineage and freeze evidence

Metadata makes local net zero emissions, sector decarbonisation & intervention prioritisation intelligence reproducible. This folder currently contains guidance; no acquisition manifest or source sign-off is claimed.

## Required records after acquisition

- Source manifest: source ID, exact/resolved URL, retrieval UTC, actual release, filename, bytes, SHA-256, archive members/sheets and coverage.
- Publisher methodology and licence/attribution evidence with provenance and retrieval date.
- Schema and field dictionary: name, type, meaning, units, key role, missing/suppression markers and valid values.
- Business glossary and critical data elements, with named steward and approved definitions.
- Grain, hierarchy and join-cardinality documentation.
- Field-level lineage from raw fields through transformations to each headline metric/dashboard measure.
- Quality profile, row-accounting reconciliation, exclusions, unresolved exceptions and their decision impact.
- Freeze approval, change log and later revision comparisons.

## Model contract

Year × local-authority code × sector/subsector × gas/CO2e basis × territorial or within-influence scope. Keep source totals and subsector details at separate hierarchy levels.

## Metric definition coverage

- Emissions: Published emissions in the workbook's stated unit and gas/CO2e scope.
- Sector share: 100 × compatible sector emissions / matching authority total; avoid double counting subsectors.
- Change since 2005: Current minus 2005 emissions, with percentage change only for a valid positive base.
- Recent five-year change: 2024 minus 2019 emissions, subject to compatible boundaries and actual availability.
- Per-capita emissions — conditional: Emissions / compatible published population where present; state conversion to tonnes per person.
- Locally influenceable share — conditional: 100 × within-influence emissions / compatible territorial emissions where both definitions are supported.
- Reduction contribution: Sector absolute reduction / total authority reduction, with sign and near-zero-total caveats.
- Coverage: Valid comparable LA/sector/year cells / expected selected cohort cells.

Every listed metric needs source fields, transformation/formula, valid grain, unit, numerator/denominator, exclusions, zero/missing behaviour, refresh expectation, owner and test reference. Mark conditional metrics unavailable if the actual source cannot support them.

Store actual evidence only; never invent publisher schema, a completed licence review, a checksum or a stakeholder approval. See [source register](../SOURCE_REGISTER.md) and [acceptance criteria](../../project/ACCEPTANCE_CRITERIA.md).
