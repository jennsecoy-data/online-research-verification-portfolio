# Research Findings Brief: Recommended Source Hierarchy for Business Verification

## Portfolio Sample Disclaimer

This independent portfolio sample was created using publicly available information.

It was not commissioned by, reviewed by, or affiliated with Chewy, Inc., the U.S. Securities and Exchange Commission, or the Wikimedia Foundation.

Conclusions are intended for general research and data-quality purposes and are not legal or investment advice.

## Research Details

| Field | Entry |
|---|---|
| Researcher | Jennifer Secoy |
| Date reviewed | 2026-08-04 |
| Research question | Which public sources should researchers prioritize when verifying business information? |
| Case example | Chewy, Inc. |
| Intended audience | Research, data-quality, documentation, compliance-support, and business-operations teams |
| Research period | August 4, 2026 |
| Overall confidence | High |

## Executive Summary

Business information should not be accepted solely because it appears on a familiar or highly ranked webpage.

Different sources are authoritative for different types of information.

Using Chewy as a case example, this review found that:

1. Regulatory filings are the strongest source for legal entity information, incorporation, principal executive office, corporate filing telephone number, stock symbol, and exchange.
2. Official company websites are generally strongest for current products, services, customer-support channels, and public contact information.
3. Investor-relations pages are useful for annual reports, SEC filings, investor contacts, and company-approved corporate descriptions.
4. Terms such as “headquarters,” “co-headquarters,” “corporate hub,” and “principal executive office” should not automatically be treated as interchangeable.
5. Wikipedia and similar reference sources can support discovery but should not be the final authority for database updates or formal verification.
6. Conflicting information should be preserved and labeled by purpose rather than overwritten without investigation.

The recommended approach is to match each data field to the source best qualified to support it.

## Research Objective

The objective was to develop a practical source hierarchy for verifying public business information.

The review focused on determining:

- Which sources should be treated as authoritative
- Which sources are appropriate only for supporting research
- How researchers should handle conflicting location and contact information
- How information should be labeled before entry into a structured database
- When additional verification is required

## Scope

### Included

The review included:

- Legal business name
- State of incorporation
- Principal executive office
- Headquarters descriptions
- Corporate and customer-service contact information
- Products and services
- Public-company reporting
- Source authority
- Source currency
- Source purpose
- Cross-source consistency

### Excluded

The review did not include:

- Private corporate records
- Paid business-information databases
- Direct contact with Chewy
- Physical address verification
- Legal entity verification for subsidiaries
- Financial analysis
- Investment recommendations
- Review of every online directory or social-media profile

## Methodology

1. Define the business information requiring verification.
2. Review the company’s current SEC Form 10-K.
3. Review the company’s official investor-relations resources.
4. Review the company’s official customer-facing website.
5. Compare location, contact, identity, and service information across sources.
6. Identify differences in terminology and intended use.
7. Evaluate the authority and currency of each source.
8. Assign each source type an appropriate role in the verification process.
9. Develop recommendations for database entry and discrepancy handling.

## Key Findings

| Finding | Supporting evidence | Confidence | Business impact |
|---|---|---|---|
| Regulatory filings are strongest for legal and registrant information | Chewy’s Form 10-K identifies its legal name, state of incorporation, principal executive office, corporate filing phone number, stock symbol, and exchange | High | Reduces errors in legal-name, corporate-address, and public-company fields |
| Official websites are strongest for customer-facing information | Chewy’s official website describes current products, services, customer care, and corporate inquiry channels | High | Prevents the use of a regulatory contact for routine customer service |
| Multiple location descriptions may all be valid | The SEC filing lists a principal executive office in Plantation, while Chewy’s investor FAQ describes co-headquarters in Florida and Massachusetts | High | Locations should be labeled by function rather than treated as duplicates |
| Phone numbers must be stored by purpose | Corporate filing and customer-service sources display different telephone numbers | High | Prevents misrouting calls and incorrect contact records |
| Reference sources should not replace original evidence | Wikipedia is collaboratively edited and summarizes information from other sources | High | Important claims should be traced to the cited original source |
| Source selection should be field-specific | No single source is best for every type of business information | High | Improves accuracy and supports defensible research decisions |

## Detailed Findings

### Finding 1: Regulatory Filings Should Lead Legal-Entity Verification

Chewy’s Form 10-K identifies:

- The registrant as Chewy, Inc.
- Delaware as the jurisdiction of incorporation
- 7700 West Sunrise Boulevard, Plantation, Florida 33322 as the principal executive office
- 786-320-7111 as the registrant telephone number
- CHWY as the Class A common-stock symbol
- The New York Stock Exchange as the applicable exchange

These fields are presented as formal registrant information in a filing submitted to the U.S. Securities and Exchange Commission.

For public-company research, the most current applicable SEC filing should generally be prioritized for:

- Exact legal entity name
- State or jurisdiction of incorporation
- Principal executive office
- Registrant telephone number
- Trading symbol
- Stock exchange
- Filing status
- Financial reporting periods

**Research decision:**

Use the SEC filing as the primary source for formal public-company and registrant fields.

### Finding 2: Official Company Pages Should Lead Customer-Facing Verification

Chewy’s official website describes its current business offerings, including:

- Pet products
- Pharmacy services
- Veterinary guidance
- Veterinary care
- Customer support
- Autoship
- Corporate inquiry channels

This information is more appropriate for customer-facing and operational fields than an SEC cover page.

Official company pages should generally be prioritized for:

- Current products and services
- Customer-support channels
- Public corporate email addresses
- Program descriptions
- Store or service availability
- Customer policies
- Public-facing brand information

**Research decision:**

Use the official company website for current operational and customer-facing information, while recognizing that promotions and service descriptions may change more frequently than regulatory records.

### Finding 3: Location Terms Must Be Preserved With Context

The SEC filing identifies a principal executive office in Plantation, Florida.

Chewy’s investor-relations FAQ describes the company as having co-headquarters in Florida and Massachusetts.

These statements are not necessarily contradictory.

A company may use several terms for different purposes, including:

- Principal executive office
- Legal address
- Corporate headquarters
- Co-headquarters
- Corporate hub
- Mailing address
- Registered-agent address
- Operational location

Flattening all of these into one generic “headquarters” field could create an inaccurate record.

**Research decision:**

Store each location in a field that preserves its stated purpose.

Recommended fields may include:

| Field | Example use |
|---|---|
| Principal executive office | Address identified in a regulatory filing |
| Corporate headquarters | Location identified by the company as its headquarters |
| Co-headquarters | Multiple headquarters locations identified by the company |
| Registered address | Legal registration or registered-agent address |
| Additional corporate location | Other verified offices or corporate hubs |

### Finding 4: Contact Information Should Be Labeled by Function

A public company may publish different contact information for:

- Customer service
- Corporate inquiries
- Investor relations
- Media inquiries
- Vendors
- Affiliates
- Regulatory filings
- Physical office reception

The presence of multiple phone numbers or email addresses does not automatically indicate an error.

For example, a registrant telephone number shown in an SEC filing should not automatically replace the company’s customer-service number.

**Research decision:**

Each contact should be stored with a contact type and source.

Recommended contact fields include:

| Contact type | Intended purpose |
|---|---|
| Customer-service phone | Customer account, order, and product support |
| Corporate phone | General corporate or registrant contact |
| Corporate email | Company and mission inquiries |
| Investor-relations email | Shareholder and financial-reporting questions |
| Media email | Press and media inquiries |
| Vendor contact | Supplier and partner communication |

### Finding 5: Reference Sources Are Useful for Discovery, Not Final Verification

Wikipedia can provide:

- A general company overview
- Historical context
- Names and dates requiring further research
- Links to articles, filings, and other sources
- A starting point for unfamiliar topics

However, Wikipedia is collaboratively edited, and the article itself is not the original source for the information it summarizes.

A cited statement should be traced back to the linked source whenever the information will be used for:

- Formal verification
- Client deliverables
- Database updates
- Compliance decisions
- Legal-entity research
- Financial reporting
- High-risk operational decisions

**Research decision:**

Use Wikipedia and similar sources as research leads or supporting context only.

## Recommended Source Hierarchy

The appropriate hierarchy depends on the data point being researched.

| Priority | Source type | Recommended use |
|---|---|---|
| 1 | Government filing or official registry | Legal entity, incorporation, regulatory status, formal addresses, licenses, and filings |
| 2 | Official company investor-relations or governance page | Annual reports, SEC filings, leadership, investor contacts, and company-approved corporate information |
| 3 | Official company customer-facing website | Current services, products, support contacts, locations, policies, and programs |
| 4 | Government or regulator guidance | Regulatory interpretation, requirements, deadlines, and agency procedures |
| 5 | Reputable news or industry publication | Independent context, recent developments, and events requiring confirmation |
| 6 | Professional directory or database | Supplemental research leads that should be independently verified |
| 7 | Wikipedia or general reference source | Background information and discovery of original sources |
| 8 | Social media, forums, or user-generated content | Leads, public sentiment, or claims requiring substantial verification |

## Field-to-Source Decision Guide

| Data field | Preferred source |
|---|---|
| Legal business name | Government registry or regulatory filing |
| State of incorporation | Government registry or regulatory filing |
| Principal executive office | Current regulatory filing |
| Stock symbol and exchange | SEC filing or official investor-relations page |
| Annual report | SEC or official investor-relations page |
| Customer-service phone | Official customer-support page |
| Corporate email | Official company contact page |
| Products and services | Official company website |
| Current promotion | Official offer page and applicable terms |
| Company history | Official history page supported by independent sources |
| Headquarters description | Regulatory filing and official corporate pages, with terminology preserved |
| Operating status | Multiple current authoritative sources |
| Reputation or customer sentiment | Independent review and news sources, clearly labeled as opinion or experience |

## Discrepancies and Open Questions

| Topic | Issue identified | Research decision | Follow-up needed |
|---|---|---|---|
| Principal office versus co-headquarters | Sources use different location terminology | Preserve both descriptions and label their function | None unless the client requires one headquarters field |
| Corporate versus customer-service phone | Different numbers serve different purposes | Store separately with contact type | Verify the intended use before contacting |
| Brand name versus legal name | “Chewy” and “Chewy, Inc.” may appear in different contexts | Use the legal name for entity records and the brand name for public-facing records | Confirm database field definitions |
| Current services | Official pages may change as offerings expand | Record the date accessed | Recheck before time-sensitive publication |
| Reference-source claims | Some claims may rely on older citations | Trace claims to the original source | Replace unsupported or outdated information |

## Source Log

| Source | Source type | Date accessed | Information supported | Reliability |
|---|---|---|---|---|
| https://www.sec.gov/Archives/edgar/data/1766502/000176650226000034/chwy-20260201.htm | Government regulatory filing | 2026-08-04 | Legal name, incorporation, principal executive office, registrant phone, ticker, and exchange | High |
| https://investor.chewy.com/financials/annual-reports/default.aspx | Official investor-relations website | 2026-08-04 | Current and archived annual-report access | High |
| https://investor.chewy.com/resources/investor-faqs/default.aspx | Official investor-relations website | 2026-08-04 | Investor contact information and corporate location description | High |
| https://www.chewy.com/app/content/about-us | Official company website | 2026-08-04 | Current products, services, customer care, and corporate contact information | High |
| https://en.wikipedia.org/wiki/Wikipedia | Collaborative encyclopedia | 2026-08-04 | Platform structure, editing model, and content policies | Moderate for platform description |

## Limitations

This research was limited to publicly accessible online sources.

The review did not include:

- Direct confirmation from Chewy
- Paid corporate-registration databases
- State-level registration records
- Historical address research
- Physical office verification
- Subsidiary-level research
- Review of every customer-support page
- Evaluation of third-party business directories
- Legal interpretation of corporate terminology

Webpages and company information may change after the review date.

## Final Assessment

**Overall confidence:** High

**Conclusion:**

Reliable business verification requires matching each data field to the source most qualified to support it.

No single webpage should be treated as universally authoritative.

Regulatory filings should lead formal public-company and legal-entity research. Official company pages should lead customer-facing and operational research. Reference sources may assist discovery but should not replace original evidence.

**Recommendation:**

Research and data-quality teams should implement a field-specific source hierarchy and require researchers to record:

1. The information found
2. The source type
3. The date accessed
4. The intended purpose of the information
5. Any conflicting values
6. The final research decision
7. The confidence level
8. Any required follow-up

Conflicting information should be investigated and labeled rather than automatically overwritten.
