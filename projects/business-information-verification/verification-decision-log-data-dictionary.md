# Verification Decision Log Data Dictionary

## Purpose

This document defines the fields, accepted values, and data-quality rules used in the structured business verification decision log.

The decision log preserves both the original information found in a source and the normalized value recommended for structured use. It also documents verification status, confidence, source type, and the reasoning behind each research decision.

## Related File

[Business Verification Decision Log](sample-verification-decision-log.csv)

## Field Definitions

| Field | Data type | Required | Description | Example |
|---|---|---:|---|---|
| `record_id` | Text | Yes | Unique identifier assigned to each verification decision | `CVS-004` |
| `company` | Text | Yes | Public-facing company or organization associated with the record | `CVS Health` |
| `field_name` | Text | Yes | Standardized name of the data field being verified | `published_corporate_phone` |
| `source_value` | Text | Yes | Information exactly as found in the reviewed source | `1-800-746-7287` |
| `normalized_value` | Text | Yes | Standardized value recommended for structured use | `800-746-7287` |
| `source_type` | Text | Yes | Category describing the authority or purpose of the source | `SEC filing` |
| `source_url` | URL | Yes | Direct link to the reviewed source | `https://www.sec.gov/...` |
| `date_accessed` | Date | Yes | Date the source was reviewed, formatted as `YYYY-MM-DD` | `2026-08-04` |
| `verification_status` | Controlled text | Yes | Final research decision for the data point | `Verified with context` |
| `confidence` | Controlled text | Yes | Confidence assigned to the research decision | `High` |
| `quality_note` | Text | Yes | Explanation of normalization, discrepancies, limitations, or intended field use | `Stored separately from the SEC registrant phone.` |

## Verification Status Values

| Value | Definition |
|---|---|
| `Verified` | The value is supported by an authoritative source and requires no significant qualification |
| `Verified with normalization` | The source value is supported, but formatting was standardized for structured use |
| `Verified with context` | The source value is supported, but its meaning, purpose, or relationship requires explanation |
| `Partially Verified` | Some elements are supported, but one or more details remain uncertain |
| `Unable to Verify` | Available sources do not provide enough reliable evidence |
| `Conflicting` | Authoritative sources provide materially different values that cannot yet be reconciled |

## Confidence Values

| Value | Definition |
|---|---|
| `High` | Supported by a current authoritative source, with no unresolved material conflict |
| `Moderate` | Supported by credible evidence, but affected by age, indirect sourcing, or limited corroboration |
| `Low` | Based on incomplete, outdated, conflicting, or weak evidence |

## Source-Type Examples

Recommended source-type labels include:

- Government regulatory filing
- Government registry
- Official company website
- Official investor-relations website
- Official customer-support page
- Official careers website
- Official policy or terms page
- Reputable news publication
- Industry publication
- Professional directory
- Collaborative reference source
- Other public source

Specific labels such as `SEC filing` may be used when they communicate the source more clearly.

## Normalization Rules

### Business Names

- Preserve the exact legal name in `source_value`.
- Remove no legal suffixes from the normalized legal-entity field.
- Keep public-facing brands separate from legal entities.
- Document parent-company and brand relationships in `quality_note`.

### Addresses

- Preserve the source wording in `source_value`.
- Standardize state names to postal abbreviations when appropriate.
- Retain apartment, suite, building, and directional information.
- Do not combine separate locations unless the field is specifically designed for multiple locations.
- Distinguish principal executive offices, headquarters, mailing addresses, registered-agent addresses, and additional corporate locations.

### Telephone Numbers

- Preserve the published format in `source_value`.
- Use a consistent normalized format.
- Store customer-service, corporate, investor, regulatory, and brand-specific numbers separately.
- Do not assume two phone numbers are conflicting until their intended purposes are compared.

### Dates

- Use `YYYY-MM-DD`.
- Record the date the source was reviewed, not the date the CSV was edited.
- Keep filing dates, effective dates, review dates, and publication dates in separate fields when applicable.

### URLs

- Link directly to the reviewed page or filing when possible.
- Prefer official and authoritative sources.
- Avoid tracking parameters when a clean source URL is available.
- Do not replace a source URL with a general homepage when a specific supporting page exists.

### Brands and Business Units

- Do not treat a parent company, subsidiary, brand, service, or operating segment as interchangeable.
- Preserve the relationship in the normalized value or quality note.
- Use a legal-entity field only for the verified legal entity.

## Data-Quality Checks

Before a record is considered complete, verify that:

1. `record_id` is unique.
2. No required field is blank.
3. `date_accessed` uses the correct date format.
4. `source_url` opens to the intended source.
5. `source_value` preserves the original information.
6. `normalized_value` follows the documented formatting rules.
7. `verification_status` uses an approved value.
8. `confidence` uses an approved value.
9. `quality_note` explains every contextual, normalized, or conflicting decision.
10. Contact information is labeled by purpose.
11. Corporate relationships are not flattened into one entity.
12. The selected source is appropriate for the field being verified.

## Example Research Decision

| Field | Example |
|---|---|
| Company | CVS Health |
| Field being verified | Corporate telephone number |
| Source value | `1-800-746-7287` |
| Normalized value | `800-746-7287` |
| Verification status | Verified |
| Confidence | High |
| Quality note | Published corporate headquarters number; stored separately from the SEC registrant telephone number |

## Limitations

The decision log documents research findings as of the recorded access date.

A verified value may later change because of:

- New regulatory filings
- Address or contact updates
- Corporate restructuring
- Brand changes
- Website revisions
- Updated annual reports
- Corrections to public records

Time-sensitive records should be rechecked before use in a new client deliverable or database update.
