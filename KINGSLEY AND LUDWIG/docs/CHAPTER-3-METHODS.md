# Chapter 3: Research Methodology

## 3.1 Research Approach and Design

This study uses an exploratory, cross-sectional questionnaire design to compare reported risk exposures associated with in-house, outsourced and hybrid operating arrangements. The research is descriptive and comparative. It examines professional assessments collected during a defined period; it does not use experimental manipulation or longitudinal observation and cannot establish that an operating model causes a particular risk outcome.

The analysis follows this organising sequence:

**Operating model → Resource configuration → Control distribution → Dependency structure → Risk exposure → Consequences → Response and recovery → Residual risk.**

This sequence is a conceptual framework for organising the investigation. It is not a causal model tested by the dataset.

## 3.2 Unit of Assessment and Scope

The unit of assessment is one specific operational activity within the respondent's organisation. Respondents were asked to select one representative activity they were sufficiently familiar with and assess the operating model used for that activity. The study does not assume that an organisation uses the same operating model across all functions.

The activity options in the response export are Production or service delivery; IT or technology services; Maintenance or asset management; Logistics or facilities; Procurement or supply chain; and Supply chain or logistics. The last two categories are separate response options and are retained separately in the analysis.

The operating-model categories are Predominantly in-house, Predominantly outsourced and A combination of in-house and outsourced. The latter is referred to as hybrid in the analysis.

## 3.3 Operationalisation of Variables

The response export contains 29 columns: one sequential record identifier (`profile_id`) and 28 survey variables. The variables cover respondent and organisational context, the assessed activity, the operating model, model-specific ratings and risks, common resilience ratings, failure consequences, make-or-buy factors and perceived overall risk effect.

| Code | Variable | Measurement / analysis |
|---|---|---|
| A1 | Country | Categorical |
| A2 | Industry | Categorical |
| A3 | Role or function | Categorical, self-reported |
| A4 | Knowledge level | Categorical, self-reported familiarity/responsibility |
| A5 | Company size | Employee-size band |
| B1 | Activity | Categorical; unit of assessment |
| B2 | Operating model | Categorical; primary grouping variable |
| IH1 | Internal skill dependency | Ordinal rating, 1–10 |
| IH2 | Internal control effectiveness | Ordinal rating, 1–10 |
| IH3 | Internal resource disruption impact | Ordinal rating, 1–10 |
| IH4 | Internal scalability | Ordinal rating, 1–5 |
| IH5 | Primary in-house risk | Categorical |
| OS1 | Supplier dependency | Ordinal rating, 1–10 |
| OS2 | Supplier monitoring effectiveness | Ordinal rating, 1–10 |
| OS3 | Supplier disruption impact | Ordinal rating, 1–10 |
| OS4 | Provider replacement ease | Ordinal rating, 1–5 |
| OS5 | Primary outsourcing risk | Categorical |
| HY1 | Responsibility clarity | Ordinal rating, 1–10 |
| HY2 | Cross-boundary information effectiveness | Ordinal rating, 1–10 |
| HY3 | Handoff effectiveness | Ordinal rating, 1–10 |
| HY4 | Primary hybrid risk | Categorical |
| D1 | Problem-detection effectiveness | Ordinal rating, 1–10 |
| D2 | Recovery effectiveness | Ordinal rating, 1–10 |
| D3 | Accountability clarity | Ordinal rating, 1–10 |
| D4 | Failure consequences | Multiple selection |
| E1 | Make-or-buy factors | Multiple selection |
| E2 | Perceived overall risk effect | Categorical |
| E3 | Additional insight | Optional open text |

The model-specific ratings are asked only within the corresponding branch. IH2, OS2 and HY1–HY3 relate to governance but measure different constructs and are not combined into a common control score. The 1–5 and 1–10 rating formats are also kept separate.

The response export stores the selected rating values as numbers. Because these are ordinal response formats, means and sample standard deviations are used as descriptive summaries alongside medians and ranges. They are not treated as proof that the distance between all response categories is equal.

## 3.4 Sampling Strategy and Respondent Eligibility

The study used purposive, non-probability recruitment. The intended respondents were people with operational responsibility, management or supervision experience, procurement or supply-chain responsibility, or professional experience with the activity being assessed.

The researchers' recruitment records describe a staged pool of approximately 300 prospective contacts in Finland and 400 across 11 other European countries. The stated sourcing channels included Finnish and European corporate registries, B2B industry directories, professional industrial-management associations and targeted direct outreach. Screening criteria included role relevance, visibility of the assessed activity and a corporate email address. The researchers report excluding generic addresses such as info@ and sales@ from the qualified contact lists.

The approximate 700 contacts represent the staged lead pool, not a verified count of invitations delivered. The number of eligible invitations, delivered messages, bounces and opt-outs is not available in the response export. A response rate is therefore not calculated.

The thesis plan set a minimum target of 25 usable responses and a preferred range of 30–40. The final export contains 30 respondent records. The questionnaire did not collect a verified organisation identifier; the records cannot be described as 30 unique organisations.

The current response export contains the following self-reported familiarity categories: directly responsible (11), manage or supervise (11), support decisions (4), and professional experience (4). These categories describe respondents' reported involvement and are not independent verification of their professional competence.

## 3.5 Questionnaire and Data Collection

The questionnaire was hosted on Tally at https://tally.so/r/RGXG6j. It collected respondent context, the assessed activity, the operating model and ratings relevant to the selected operating-model branch, followed by common questions on problem detection, recovery, accountability, failure consequences, make-or-buy factors and perceived overall risk effect.

Tally supports conditional logic to show or hide questions and route respondents according to previous answers. The researchers' implementation records state that the questionnaire used conditional paths for the three operating-model categories. The final response export is consistent with this structure: in-house branch fields are populated for in-house records, outsourced branch fields for outsourced records, and hybrid branch fields for hybrid records. The export alone does not verify the exact published form configuration or every test scenario. Tally's own guidance recommends reviewing conditions and testing different answer paths before deployment (Tally 2026).

### 3.5.1 Pilot Testing

The researchers' project records state that four practitioners pre-tested the instrument before wider distribution:

- Operations Director, manufacturing, Finland.
- Head of Procurement / Supply Chain, industrial services.
- Quality Assurance Lead, technology / engineering.
- Maintenance / Logistics Manager.

The reported completion duration was approximately 6–8 minutes. The pilot notes report no observed drop-off and identify three refinements: clarifying the instruction to assess one representative core operational activity; adding verbal anchors to D1 problem detection, D2 recovery effectiveness and D3 accountability clarity; and refining the wording of IH5, OS5 and HY4 primary-risk options.

The final IH5, OS5 and HY4 values in the response export are Staff Shortage Risk, Single-Point Skill Risk, Supplier Performance Risk, Single Supplier Risk and Coordination Failure Risk. The four-person pilot supports reporting that practitioner pre-testing and wording refinement occurred. It does not establish statistical reliability, construct validity or population-wide usability. AAPOR recommends pre-testing questionnaires and piloting survey procedures to identify interpretation and administration problems (AAPOR 2022).

The pilot details are attributed to researcher-provided project records. The original pilot worksheets were not present in the repository snapshot reviewed.

## 3.6 Data Processing and Analysis

The current source export contains 30 records and 29 columns. The source file `DATA/responses.csv` is retained unchanged. A separate analysis copy, `DATA/responses-readable.csv`, uses readable column labels and leaves the 30 N/A placeholders in the optional additional-insight field blank. Other response values and record order are preserved. The data dictionary is `DATA/DATA-DICTIONARY.md`.

### 3.6.1 Branch Applicability and Completeness

The questionnaire routes respondents to one of three model-specific branches:

- IH1–IH5 apply to the 9 in-house records.
- OS1–OS5 apply to the 12 outsourced records.
- HY1–HY4 apply to the 9 hybrid records.

Blank cells in branches not shown to a respondent are structurally not applicable. All branch-specific closed-ended fields are populated for the respondents to whom they apply. Common closed-ended fields are populated for all 30 records.

The optional E3 field contains the literal value N/A in all 30 source records. It provides no usable narrative response. No qualitative coding, themes or quotations are reported from E3.

### 3.6.2 Descriptive Analysis

The analysis uses:

- Counts and percentages for categorical variables, with the denominator stated.
- Counts and within-group percentages for primary-risk categories.
- Means, medians, sample standard deviations and ranges for rating items, with the applicable subgroup size stated.
- Cross-tabulations of operating model with assessed activity, failure consequences and E2 perceived overall risk effect.
- Respondent-level frequencies for multiple-selection questions.

D4 and E1 are multiple-selection items. Percentages can therefore exceed 100% when added. For E1, Cost and Total cost are grouped as Cost and financial considerations; Control and Direct control are grouped as Control and operational authority. Each respondent is counted once per harmonised category. The original response labels remain unchanged in the source data.

No inferential statistical tests or causal estimates are reported. The subgroup sizes are 9, 12 and 9, and the sample is non-probability based. Results are interpreted descriptively.

## 3.7 Research Ethics and Data Protection

The researchers report that a participant information notice was included in the Tally questionnaire and that supervisor permission to proceed was obtained. No formal ethics-review decision is documented in the materials reviewed for this revision. This chapter does not claim ethics-committee approval.

The exact participant notice, completed data-management plan, platform configuration, and records of access, retention and disposal were not available in the repository snapshot reviewed. Claims about the legal basis for processing, collection of technical metadata, separation of contact data, storage security or deletion arrangements must be checked against those records before submission.

The response export does not contain names. However, combinations of country, industry, role, company-size band and activity may indirectly identify a respondent, especially in small or specialised sectors. The absence of names alone does not establish anonymity. The European Data Protection Board distinguishes anonymisation from pseudonymisation and notes that pseudonymised data can remain personal data where additional information can identify an individual (EDPB 2026). GDPR Article 5 sets out principles including lawfulness, transparency, purpose limitation, data minimisation, accuracy and storage limitation (European Union 2016).

Karelia UAS guidance states that a data-management plan should describe the collection, use, storage and disposal of thesis data. The researchers should ensure that the final thesis accurately reflects the completed plan and the supervisor's decision on whether a research permit or ethical review was required (Karelia UAS 2026a; Karelia UAS 2026b).

## 3.8 Methodological Limitations

The findings must be interpreted within the following limitations:

1. **Sample size:** The export contains 30 respondent records, divided into groups of 9, 12 and 9. These small groups limit the strength of comparisons.
2. **Non-probability sampling:** Purposive recruitment does not produce a probability sample and does not support population-representative estimates.
3. **Respondent and organisation count:** The dataset does not establish 30 unique organisations.
4. **Activity-specific assessment:** Each respondent assessed one activity. Results should not automatically be generalised to the respondent's entire organisation.
5. **Self-reported data:** Ratings and categories reflect respondents' assessments rather than audited incident, cost or performance records.
6. **Cross-sectional design:** The data do not establish temporal change or causal effects.
7. **Measurement:** Rating items are ordinal. Means are reported as descriptive summaries alongside medians. Branch-specific governance measures are related but not identical.
8. **Qualitative material:** E3 contains N/A in all 30 records, so no qualitative analysis is supported.
9. **Data protection evidence:** The participant notice and data-management records must be checked before making claims about anonymity, GDPR compliance or specific security controls.

The study therefore provides an exploratory description of the responses collected. It does not prove that one operating model causes a particular risk outcome or represents all European organisations.

## References

American Association for Public Opinion Research (AAPOR). 2022. Best Practices for Survey Research. https://aapor.org/standards-and-ethics/best-practices/. Accessed 5 November 2026.

European Data Protection Board (EDPB). 2026. Anonymisation / pseudonymisation. https://www.edpb.europa.eu/topics/ai-and-technology/anonymisation-pseudonymisation_en. Accessed 5 November 2026.

European Union. 2016. Regulation (EU) 2016/679 (General Data Protection Regulation). https://eur-lex.europa.eu/eli/reg/2016/679/. Accessed 5 November 2026.

Karelia University of Applied Sciences. 2026a. Thesis Instructions: Data Management Plan. https://libguides.karelia.fi/c.php?g=689495&p=5202279. Accessed 5 November 2026.

Karelia University of Applied Sciences. 2026b. Thesis Instructions: Report Outline. https://libguides.karelia.fi/c.php?g=689495&p=4935741. Accessed 5 November 2026.

Tally. 2026. Conditional Logic. https://tally.so/help/conditional-form-logic. Accessed 5 November 2026.
