# Chapter 4: Implementation

## 4.1 Chronological Implementation Stages

The study was implemented by a two-researcher team. The project records supplied for this revision identify six stages between early October and 30 October 2026. Dates below are reported at the level of detail available in those records; exact dispatch and completion timestamps are not available in the materials reviewed.

| Stage | Reported timeframe | Activities and outputs |
|---|---|---|
| Instrument design and setup | Early to mid-October 2026 | Questionnaire prepared, conditional paths configured in Tally, and participant information notice included. Survey link: https://tally.so/r/RGXG6j |
| Pilot review | Mid-October 2026 | Four practitioners pre-tested the instrument. Reported completion duration was approximately 6–8 minutes. Wording and routing observations were recorded. |
| Recruitment-pool staging | Mid-October 2026 | Approximately 300 Finnish and 400 wider-European prospective contacts were staged in two lead lists. |
| Phased outreach and response collection | Mid- to late-October 2026 | Invitations were sent in waves. The final response export contains 30 records, with 12 Finland-based and 18 from 11 other European countries. |
| Data audit and quality control | Late October 2026 | Response schema, conditional-branch fields, categories and response-level counts were checked. |
| Dataset freeze and reporting | 30 October 2026 | The response export was designated as the frozen dataset and used for descriptive analysis and thesis reporting. |

The pilot and recruitment details in this chapter are based on the researchers' project records supplied for this revision. The lead-list files, pilot worksheets and message-dispatch logs were not present in the repository snapshot reviewed. The stated project details are therefore documented as researcher records, not independently audited third-party evidence.

## 4.2 Questionnaire Construction and Pilot Testing

The questionnaire was implemented in Tally at https://tally.so/r/RGXG6j. It asked respondents to assess one representative operational activity in their organisation. This instruction addressed the possibility that one organisation may use different operating models across different functions.

### 4.2.1 Pilot participants

The project records identify four practitioners who pre-tested the instrument before wider distribution:

- Operations Director, manufacturing, Finland.
- Head of Procurement / Supply Chain, industrial services.
- Quality Assurance Lead, technology / engineering.
- Maintenance / Logistics Manager.

The records describe the participants as senior industry practitioners. The available notes do not provide participant names, exact test dates, or a separate record of their eligibility screening. Pilot participants are not included as additional observations in the 30-record response export unless separately identified; the export itself contains 30 records and does not identify pilot status.

### 4.2.2 Pilot observations and refinements

The pilot notes report a completion duration of approximately 6–8 minutes across the four testers and no observed drop-off during the pilot. The notes also record the following refinements:

1. **Activity-specific assessment:** The Section B instruction was clarified to ask respondents to select and assess one representative core operational activity, rather than treating the organisation as if it had only one operating model.
2. **Rating-scale anchors:** The D1 problem-detection, D2 recovery-effectiveness and D3 accountability-clarity scales were given explicit verbal anchors, from 1 (Very Low / Ineffective) to 10 (Very High / Highly Effective).
3. **Risk-category wording:** The primary vulnerability options in IH5, OS5 and HY4 were refined to use operational terminology. The final export records the categories Staff Shortage Risk, Single-Point Skill Risk, Supplier Performance Risk, Single Supplier Risk and Coordination Failure Risk.

The four-person pre-test provides evidence that the instrument was reviewed by practitioners and that wording changes were made. It does not establish statistical reliability, construct validity, or population-wide usability. Questionnaire pre-testing is intended to identify interpretation and administration problems; a small pilot should not be represented as psychometric validation (AAPOR 2022).

## 4.3 Recruitment Pool and Sampling

The researchers used purposive recruitment directed at people with operational responsibility, management or supervision experience, procurement or supply-chain responsibility, or professional experience with the activity being assessed.

The supplied recruitment records describe the following sourcing channels: Finnish and European corporate registries, B2B industry directories, professional industrial-management associations and targeted direct outreach. Screening criteria included relevant role or activity visibility and a corporate email address. Generic addresses such as info@ and sales@ were excluded from the qualified contact lists.

Two lead lists were staged:

- Finland: approximately 300 prospective contacts, identified in the project records as `leads_final_fi_300`.
- Wider Europe: approximately 400 prospective contacts across 11 countries, identified as `leads_final_eu_400`.

The combined staged pool was approximately 700 prospective contacts. This is a lead-pool size, not a verified number of delivered invitations or a response-rate denominator. The exact number of invitations sent, delivery failures, opt-outs and unique eligible contacts cannot be calculated from the 30-row response export.

The recruitment approach was purposive and non-probability based. The geographic composition of the achieved response set was 12 respondents in Finland (40.0%) and 18 respondents in 11 other European countries (60.0%). This matches the stated 40/60 planning split in the achieved sample. The response export confirms the distribution; it does not, by itself, establish how closely the invitation process followed quotas.

## 4.4 Response Set and Participant Profile

The frozen export contains 30 respondent records and 29 columns: one sequential record identifier and 28 survey variables. It contains responses from 12 countries in Europe: Finland (12), Germany (2), Sweden (3), Spain (2), France (2), Italy (1), the Netherlands (2), Belgium (1), Poland (2), the United Kingdom (1), Norway (1) and Denmark (1).

The term “respondent record” is used throughout. The questionnaire did not collect a verified organisation identifier, so the dataset does not establish that the 30 respondents represent 30 unique organisations.

The operating-model distribution is:

| Operating model for the assessed activity | n | % |
|---|---:|---:|
| Predominantly in-house | 9 | 30.0% |
| Predominantly outsourced | 12 | 40.0% |
| A combination of in-house and outsourced | 9 | 30.0% |
| **Total** | **30** | **100.0%** |

The achieved sample therefore contains all three operating-model groups. The subgroup sizes remain small and are not treated as representative population samples.

## 4.5 Data Audit and Completeness

The source export contains 30 records and 29 columns. The audit distinguished between fields shown to all respondents and fields shown only within a conditional operating-model branch.

| Field group | Applicable records | Structurally non-applicable blanks |
|---|---:|---:|
| In-house branch fields (IH1–IH5) | 9 | 21 per field |
| Outsourced branch fields (OS1–OS5) | 12 | 18 per field |
| Hybrid branch fields (HY1–HY4) | 9 | 21 per field |
| Common fields and respondent context | 30 | 0 |

All branch-specific fields contain a response for each record to which that branch applies. The blanks in other operating-model branches are structurally not applicable; they are not treated as unanswered responses. The common closed-ended fields are populated for all 30 records.

The optional additional-insight field contains the literal value `N/A` in all 30 source records. This is not usable qualitative text. No thematic coding or quotation analysis was conducted from this field.

The completeness statement is therefore limited to the applicable closed-ended questions in the current export. It is not accurate to say that every one of the 29 columns contains a substantive answer for every respondent.

## 4.6 Data Preparation and Harmonisation

The source file `DATA/responses.csv` was retained as the original response export. A separate readable analysis copy was prepared at `DATA/responses-readable.csv`. The analysis copy uses descriptive column labels and leaves the 30 `N/A` placeholders in the optional additional-insight field blank. The source values and original column names remain in the source file.

The analysis used the following respondent-level harmonisation rules for the multiple-selection make-or-buy item:

- `Cost` and `Total cost` were grouped as **Cost and financial considerations**.
- `Control` and `Direct control` were grouped as **Control and operational authority**.
- Each respondent was counted once in a harmonised category, even when both original labels were selected.

The primary-risk category labels and failure-consequence labels were counted as recorded in the source export. They were not converted into a new taxonomy in the source file. The harmonised make-or-buy groupings are analytical categories and do not alter the original responses.

The analysis files are `docs/EMPIRICAL-FINDINGS-TABLES.md` and `docs/DATA-ANALYSIS-REPORT.md`. Field meanings and applicability rules are recorded in `DATA/DATA-DICTIONARY.md`.

## 4.7 Data Management and Research Ethics

The project records state that a participant information notice was included in the Tally questionnaire. The exact notice text, the completed data-management plan, the platform configuration, and the detailed storage and deletion records were not available in the repository snapshot reviewed. This chapter therefore does not claim that the study was GDPR-compliant, fully anonymous, encrypted, or stored under a particular access-control arrangement.

The absence of names in the response export does not by itself establish anonymity. Country, industry, role, company-size band and activity can form combinations that may indirectly identify a respondent, particularly in small or specialised sectors. The European Data Protection Board distinguishes anonymisation from pseudonymisation and notes that pseudonymised information can remain personal data where an individual can be identified using additional information (EDPB 2026). The researchers must describe the actual collection and handling arrangements using the participant notice and data-management records, and confirm with the supervisor whether any research permit or ethical review was required. Karelia UAS requires a data-management plan to describe collection, use, storage and disposal of thesis material (Karelia UAS 2026a; Karelia UAS 2026b).

The researchers have indicated that supervisor permission was obtained. No formal ethics-review decision is documented in the materials reviewed; this is not described as ethics-committee approval.

## 4.8 Implementation Limitations

The project records provide approximate stage windows and lead-pool sizes but do not provide exact invitation counts or dispatch dates. The response export verifies the final sample distribution but cannot independently verify the recruitment process, the pilot duration, the participant-information wording, or data-storage controls. Those claims should be retained with the project records and, where appropriate, supporting material should be included in the research archive.

The study uses a small purposive sample and self-reported assessments. Its findings are descriptive and activity-specific. They do not establish causal effects, objective incident frequencies, or population-level estimates.
