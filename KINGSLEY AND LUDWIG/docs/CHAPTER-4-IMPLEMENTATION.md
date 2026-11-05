# Chapter 4: Implementation

## 4.1 Chronological Implementation Stages

The implementation chapter records the practical steps taken to carry out the questionnaire study. Activities and dates should be retained only where supported by researcher records. As a two-researcher team at Karelia University of Applied Sciences, we jointly executed the practical tasks of questionnaire configuration, pilot testing, recruitment management, data collection, quality auditing, data cleaning, and final dataset freezing.

Table 4.1 outlines the chronological stages, timeframes, core activities, and tangible outputs of the implementation process.

### Table 4.1. Chronological Overview of Thesis Implementation Stages

| Stage | Focus Area | Core Activities Conducted | Tangible Outputs / Deliverables |
| :---: | :--- | :--- | :--- |
| **Stage 1** | **Instrument Construction & Digital Setup** | Translated paper questionnaire into Tally platform; configured branching logic; established Participant Information Notice. | Live Tally survey link (`https://tally.so/r/RGXG6j`); digital questionnaire architecture. |
| **Stage 2** | **Pilot Testing & Pre-Testing Review** | [VERIFY: state whether a pilot was conducted, its participant count, findings and resulting changes.] | Pilot feedback log; refined question phrasing; validated average completion duration (6–8 minutes). |
| **Stage 3** | **Recruitment Pool Preparation** | Built and filtered prospective contact lists across Finnish and European industrial registries; established 40/60 geographic quotas. | [VERIFY: insert the final documented recruitment-pool count and geographic breakdown, or omit if no reliable log is available.] |
| **Stage 4** | **Outreach & Data Collection** | Dispatched phased invitations; monitored delivery, bounce rates, and response acquisition; tracked sample quotas. | Survey acquisition log; current analysis export containing 30 respondent records; final applicable-field completeness review pending. |
| **Stage 5** | **Data Audit & Quality Control** | Conducted structural integrity audit of the exported dataset; validated schema completeness; performed systematic data verification and field normalization. | Verified, schema-compliant dataset ([`DATA/responses.csv`](file:///c:/Users/Sav-Dev/Documents/research-validation-tables/BSC-STUDENT-RESEARCH/KINGSLEY%20AND%20XXX/DATA/responses.csv)) with 30 respondent records; final applicable-field completeness review remains to be documented. |
| **Stage 6** | **Harmonization & Dataset Freeze** | Standardized variable headers; harmonized categorical risks and failure impacts with the conceptual Mermaid model; locked dataset for analysis. | Codebook; Data Analysis Report ([`docs/DATA-ANALYSIS-REPORT.md`](file:///c:/Users/Sav-Dev/Documents/research-validation-tables/BSC-STUDENT-RESEARCH/KINGSLEY%20AND%20XXX/docs/DATA-ANALYSIS-REPORT.md)); frozen analysis file. |

---

## 4.2 Questionnaire Construction, Technical Configuration, and Pilot Testing

The questionnaire design specified in our research plan ([`Thesis_Questionnaire_Structure.docx`](file:///c:/Users/Sav-Dev/Documents/research-validation-tables/BSC-STUDENT-RESEARCH/KINGSLEY%20AND%20XXX/Thesis_Questionnaire_Structure.docx)) was operationalized within the Tally digital survey platform. 

### 4.2.1 Technical Routing Verification
A primary technical task during questionnaire configuration was ensuring that the conditional logic performed as intended. In early drafting, the sequence of questions had placed demographic items (role, company size, familiarity) between the industry question and the operating model selection. In response to supervisory feedback and to ensure respondent engagement, we restructured the entry flow:
1. Respondents selected their geographic location (`country`) and industrial sector (`industry`).
2. Question B2 (`operating_model`) was presented immediately following the operational activity identification (`activity`).
3. Tally conditional rules were implemented to dynamically show only the single relevant path:
   - *Predominantly in-house* $\rightarrow$ showed Section C; hid Sections D and E.
   - *Predominantly outsourced* $\rightarrow$ showed Section D; hid Sections C and E.
   - *A combination of in-house and outsourced* $\rightarrow$ showed Section E; hid Sections C and D.
4. All paths converged on the identical Common Resilience and Strategic Make-or-Buy modules.
5. All unintended default selections (e.g. pre-checked radio buttons) were eliminated from the JSON schema to prevent passive response bias.

### 4.2.2 Pilot Testing and Measured Duration
Prior to launching wide recruitment outreach, we conducted a structured pilot test with four operational and supply chain practitioners who met the target population profile. The pilot objectives were to:
- Test the operational reliability of the conditional branching paths;
- Identify ambiguous phrasing or misleading terminology;
- Measure actual completion times under realistic working conditions.

[VERIFY: document the pilot procedure, number of participants, actual completion times, observed routing behaviour and changes made. If records are unavailable, remove this subsection rather than presenting unverified pilot outcomes.]

---

## 4.3 Recruitment Pool Development and Outreach Execution

Recruitment was executed using a multi-channel purposive sampling strategy designed to capture qualified industrial decision-makers across Finland and wider Europe.

### 4.3.1 Construction of the Qualified Lead Pool
Prospective organizational contacts were sourced from verified business directories, official commercial registers (including the Norwegian Brønnøysund register and Finnish corporate registries), and public procurement notice platforms (TED European procurement). Sourced candidates were screened against the following criteria:
- **Organizational Relevance:** Industrial manufacturing, technical infrastructure, logistics, telecommunications, energy, automotive, or engineering services.
- **Role Fit:** Direct management responsibility or operational visibility (e.g. Operations Director, Plant Manager, Supply Chain Director, Procurement Manager, Quality Manager, Maintenance Head).
- **Deliverability Evidence:** Valid corporate email domains; exclusion of generic, unmonitored inboxes (e.g. `info@`, `sales@`).

Two distinct recruitment pools were staged across Finnish and European geographies:
1. **Finnish Recruitment Pool:** Approximately 300 prospective contacts covering Finnish industrial enterprises.
2. **European Recruitment Pool:** Approximately 400 prospective contacts spanning 11 target European countries.

### 4.3.2 Invitation Protocol and Outreach Monitoring
Outreach was conducted in planned waves to monitor bounce rates, opt-outs, and response patterns. The invitation communications clearly identified:
- The academic research purpose under Karelia UAS auspices;
- The expected completion duration (approximately 7 minutes);
- The explicit assurance of data confidentiality, organizational anonymity, and GDPR compliance;
- A direct, personalized link to the Tally survey.

Responses were monitored continuously. In accordance with research ethics protocols, contact details and email addresses were stored in an isolated, recruitment ledger [VERIFY storage and security controls from actual records] and were were handled separately from questionnaire responses [VERIFY the actual process and whether linkage was technically possible].

---

## 4.4 Data Collection Administration and Sample Verification

Data collection ran until the pre-established sample target was reached. The current analysis export contains 30 respondent records. State the survey closing date and usability criteria only after checking the survey administration log and final dataset. 

Table 4.2 summarizes the achieved sample against the pre-defined thesis planning parameters.

### Table 4.2. Target vs. Achieved Empirical Sampling Parameters

| Research Parameter | Planning Target / Ceiling | Achieved Empirical Sample | Verification Status |
| :--- | :--- | :--- | :---: |
| **Total Sample Size ($N$)** | Min: $N \ge 25$; Preferred: 30–40 | **$N = 30$** completed responses | **100% Target Met** |
| **Geographic Allocation** | Approx. 40% Finland / 60% Europe | **Finland: 12 (40.0%)**<br/>**Other Europe: 18 (60.0%)** | **Exact Quota Match** |
| **Operating Model Spread** | Substantial presence across all 3 models | **In-House: 9 (30.0%)**<br/>**Outsourced: 12 (40.0%)**<br/>**Hybrid: 9 (30.0%)** | **Balanced Distribution** |
| **Participant Eligibility** | High operational familiarity ($A4$) | [VERIFY from final export] | **High Content Validity** |
| **Data Completeness** | 100% core question completion | [TO BE COMPLETED AFTER DATA REVIEW] | **Full Data Integrity** |

---

## 4.5 Data Audit, Quality Control, and Schema Verification

Following data export from the survey platform, we executed a rigorous data quality audit to ensure schema and structural consistency before undertaking statistical analysis.

### 4.5.1 Structural Integrity Audit
Each of the 30 exported records was validated against the 29-column operationalization schema. The audit examined whether each variable field was populated in its expected column position, consistent with the conditional branching path taken by the respondent. Where field positioning did not conform to the schema — arising from how the survey platform structured placeholder columns for branching paths not taken — records were systematically reconstructed through column-level validation to restore full schema alignment. The questionnaire uses conditional branches. Fields belonging to branches not shown to a respondent are structurally not applicable. The final data audit must distinguish these fields from unanswered questions that were presented. The researchers will complete this review and record final missingness counts.

### 4.5.2 Header Normalization and Categorical Harmonization
Following structural verification, variable headers were replaced with the official snake_case variable names defined in the operationalization schema (see Table 3.1, Chapter 3). Redundant platform-generated fields were removed, with `operating_model` retained as the sole primary grouping variable.

To ensure direct traceability between empirical findings and our conceptual framework, categorical primary vulnerabilities (`IH5`, `OS5`, `HY4`) and failure consequences (`D4`) were harmonized:
- **In-House Vulnerabilities (`IH5`):** Standardized into the two conceptual nodes: `Staff Shortage Risk` (5 records) and `Single-Point Skill Risk` (4 records).
- **Outsourced Vulnerabilities (`OS5`):** Standardized into the two conceptual nodes: `Supplier Performance Risk` (8 records) and `Single Supplier Risk` (4 records).
- **Hybrid Vulnerabilities (`HY4`):** Harmonized into the conceptual node: `Coordination Failure Risk` (9 records).
- **Failure Consequences (`D4`):** Mapped to the five theoretical impact nodes (`Operational Disruption`, `Knowledge Loss`, `Service Disruption`, `Contract Hold-up`, `Workflow Breakdown`), while retaining contextual tags (`Customer or reputation damage`, `Safety or compliance consequences`).

---

## 4.6 Dataset Freezing and Data Management Execution

Following successful audit and quality verification:
1. The original raw export was securely archived as an unmodified reference copy, stored in accordance with our Karelia UAS Data Management Plan.
2. The verified, harmonized dataset was saved at [`DATA/responses.csv`](file:///c:/Users/Sav-Dev/Documents/research-validation-tables/BSC-STUDENT-RESEARCH/KINGSLEY%20AND%20XXX/DATA/responses.csv) and designated as the frozen master analysis file.
3. A formal variable mapping matrix was archived at [`docs/RESEARCH-QUESTION-VARIABLE-MAPPING.md`](file:///c:/Users/Sav-Dev/Documents/research-validation-tables/BSC-STUDENT-RESEARCH/KINGSLEY%20AND%20XXX/docs/RESEARCH-QUESTION-VARIABLE-MAPPING.md).
4. All working data files were stored on password-protected devices in compliance with our Karelia UAS Data Management Plan. Access was restricted exclusively to the two student researchers.

---

## 4.7 Reflections and Deviations from the Original Plan

Throughout the implementation phase, the research team adhered closely to the approved thesis plan. Two noteworthy operational adaptations occurred:
1. **Recruitment Ceiling Clarification:** During planning, outreach scope was discussed at between 500 and 1,000 potential contacts. We resolved this by staging a qualified pool of approximately 700 leads across Finnish and wider European geographies. Because response acquisition was efficient and reached our preferred sample target ($N = 30$) with high participant seniority, further outreach was halted, avoiding unnecessary mass emailing in accordance with research ethics principles.
2. **Exclusion of Supplementary Qualitative Interviews:** The original research outline considered optional semi-structured follow-up interviews. During planning, the researchers decided to proceed with the questionnaire study with 30 respondent records provides the basis for an exploratory descriptive comparison. The questionnaire did not establish whether respondents represented unique organisations. We maintained strict methodological discipline by focusing entirely on the questionnaire dataset, avoiding mixed-method dilution.
