# MTL-XF-028 — Source register

**Project:** Local Net Zero Emissions, Sector Decarbonisation & Intervention Prioritisation Intelligence  
**Register date:** 16 October 2026  
**Status:** agreed source references recovered; acquisition, payload verification and freeze approval pending.

## Cohort contract

Freeze the agreed DESNZ 2005–2024 local-authority greenhouse-gas XLSX, approximately 24.9 MB in the prior agreement. Use this workbook rather than the 82.6 MB CSV. Record sheets, units, gases, revisions and territorial/within-influence definitions from actual metadata. Default analysis covers English local authorities; retain other UK areas separately for context.

## Source entries

### S1 — 2005-24-uk-local-authority-ghg-emissions.xlsx

Exact agreed download URL (copy verbatim):

```text
https://assets.publishing.service.gov.uk/media/6a3bacc7eaee00074150f326/2005-24-uk-local-authority-ghg-emissions.xlsx
```

- Publisher/source: DESNZ local/regional greenhouse-gas data tables, 2005–2024. The Excel workbook is 24.9 MB and is preferable to the 82.6 MB raw CSV for Mettelo.
- Intended role: required core input.
- Access expectation from agreement: £0, public download, no paid API required.
- Verification state: URL recovered from the final agreed conversation; browser-only retrieval on 16 October 2026 could not validate the file contents. This is not a completed download/schema/licence check.
- File acquisition state: **not downloaded or uploaded in this master-pack build**.
- Actual release/coverage, retrieval UTC, resolved URL, filename, bytes, SHA-256, sheet/archive members, row counts and schema: **pending controlled acquisition**.
- Licence and redistribution evidence: **pending inspection of the official publication and file notices**. Public accessibility alone does not establish reuse rights.
- Required before analysis: metadata and coverage validation; freeze approval by Data Governance Analyst and domain analyst.

## Acquisition manifest requirements

Create one row per acquired file, including archive members and all eight months where applicable:

`source_id, original_url, resolved_url, retrieved_utc, publisher_release, filename, bytes, sha256, format, sheets_or_members, row_count, coverage_start, coverage_end, geography, schema_version, licence_evidence_path, approved_by, approval_date`

Never enter guessed values. A missing field remains pending with an owner and reason. Source IDs above are local to this project. Preserve the actual publisher metadata and notices alongside the manifest.

## Validation and fallback

Browser checks during this build could not inspect downloadable payloads consistently; unsupported download formats and retrieval failures do not prove a URL is broken. They also do not verify schema, current availability, advertised history, size or redistribution rights. Perform a controlled file acquisition before team analysis.

If the exact link fails, locate the same release through the official publisher's publication series, record the replacement URL and compare version/coverage. Escalate any change to cohort, dimensions or reporting window through the project change log. No paid source or live API is required by the agreed design. No guarantee is made that a publisher URL will remain unchanged indefinitely.

## Data sign-off

The Data Governance Analyst and domain analyst sign the actual manifest after checking file identity, licence, coverage and definitions. Ingest only the signed cohort. Every headline metric must trace through transformations back to a registered source and field.
