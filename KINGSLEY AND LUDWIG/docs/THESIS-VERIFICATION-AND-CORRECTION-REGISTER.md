# Thesis Verification and Correction Register

**Repository:** vlthr-admin/RESEARCH-PORTFOLIOS  
**Working branch:** `audit/verified-thesis-corrections-2026-11-05`  
**Audit date:** 5 November 2026  
**Scope:** Chapters 1–6, response export, empirical tables and supporting analysis documents.

## Evidence classes and severity

- **Dataset-verified:** Recomputed directly from the current `DATA/responses.csv`.
- **Researcher-provided project record:** Supplied by the researchers for this revision. The underlying source files were not in the repository snapshot reviewed.
- **Externally verified:** Checked against an authoritative institutional, regulatory, platform or publisher source.
- **Unverified:** Insufficient evidence to retain as an established fact; removed, qualified or marked for documentary confirmation.

Severity: **Critical** = risks misrepresenting method, sample, findings, ethics or validity; **High** = materially changes interpretation; **Medium** = requires qualification; **Low** = editorial.

## Verified dataset facts

| Item | Verified result |
|---|---|
| Records | 30 respondent records |
| Columns | 29: one sequential identifier and 28 survey variables |
| Operating model | In-house 9; outsourced 12; hybrid 9 |
| Geography | Finland 12; 18 across 11 other European countries |
| Branch fields | IH1–IH5 apply to 9; OS1–OS5 apply to 12; HY1–HY4 apply to 9 |
| Branch completeness | Every applicable branch-specific closed-ended field is populated |
| Common closed-ended fields | Populated for all 30 records |
| Optional insight | 30/30 source values are literal N/A; no usable narrative text |
| Make-or-buy factors | Cost/Total cost deduplicated: 23; Control/Direct control deduplicated: 17 |
| E2 perceived risk effect | 22 report some risks decreased while others increased; 8 report risks generally increased |

The country distribution is Finland 12; Germany 2; Sweden 3; Spain 2; France 2; Italy 1; Netherlands 2; Belgium 1; Poland 2; United Kingdom 1; Norway 1; Denmark 1. The sample spans 12 European countries, not 12 EU Member States.

## Material issues and corrective actions

| ID | Severity | Issue | Verification and correction |
|---|---|---|---|
| V-01 | Critical | Treating 30 response records as 30 organisations | The export has no verified organisation identifier. Replaced with “30 respondent records”. |
| V-02 | Critical | Claiming 100% completeness across all 29 columns | Fourteen branch-specific fields are structurally blank outside the relevant route. Replaced with applicable-branch completeness. |
| V-03 | Critical | Claiming anonymity or GDPR compliance because names are absent | Indirect identification may be possible from combinations of country, industry, role, size and activity. Removed unsupported compliance/anonymity claims. |
| V-04 | High | Treating N/A in Additional Insight as qualitative evidence | All 30 source entries are N/A. Removed qualitative themes and quotations. |
| V-05 | High | Comparing branch-specific governance items as one control scale | IH2, OS2 and HY1–HY3 measure different constructs. Explicitly described them as related but non-identical. |
| V-06 | High | Describing D1 as detection speed or velocity | D1 is an effectiveness rating, not elapsed time. Corrected the wording. |
| V-07 | High | Treating E2 as objective risk change or causal effect | E2 is a perception item. Corrected throughout to “perceived overall risk effect”. |
| V-08 | High | Generalising the hybrid primary-risk result | 9/9 selected Coordination Failure Risk. Wording is limited to unanimity within this subgroup. |
| V-09 | High | Treating a four-person pilot as proof of validity or reliability | Pilot evidence supports practitioner review and wording refinement, not psychometric validation. |
| V-10 | High | Calculating a response rate using 30/700 | 700 is the staged lead-pool estimate, not a verified delivered-invitation denominator. No response rate is calculated. |
| V-11 | High | Claiming outsourcing eliminates internal resource constraints | Corrected: outsourcing changes resource allocation; client-side oversight and continuity capabilities remain relevant. |
| V-12 | High | Reporting a 2.14-point “monitoring effectiveness drop” | Internal control effectiveness and supplier monitoring effectiveness are different constructs. The subtraction is invalid as a like-for-like comparison and was removed. |
| V-13 | High | Claiming hybrid maximises recovery flexibility | D2 measures perceived recovery effectiveness. Fallback flexibility was not measured. The mechanism claim was removed. |
| V-14 | Medium | Calling the 12-country sample the European Union | United Kingdom and Norway are included. Corrected to 12 European countries / wider Europe. |
| V-15 | Medium | Combining separate activity labels | “Logistics or facilities” and “Supply chain or logistics” remain separate export categories. |
| V-16 | Medium | Treating employee-size bands as official SME classifications | Bands are reported as questionnaire categories only. |
| V-17 | Medium | Treating ordinal ratings as precise metric measurements | Means are descriptive summaries alongside medians and sample SDs; ordinal-scale limits are stated. |
| V-18 | Medium | Calling subgroups balanced or representative | Groups are 9/12/9 from purposive recruitment. Representativeness is not claimed. |
| V-19 | Medium | Adding raw Cost and Control category counts | Recomputed per respondent: 23 and 17. Original response labels remain unchanged. |
| V-20 | Medium | Using local file-system paths in repository documents | Replaced with repository-relative paths or the public survey URL. |

## Researcher-provided implementation records

The following details were supplied by the researchers on 5 November 2026 and incorporated in Chapter 4 as project-record information:

- Four pilot practitioners and their role descriptions.
- Approximate pilot completion duration of 6–8 minutes and pilot notes reporting no observed drop-off.
- Wording refinements to the activity instruction, D1–D3 anchors and IH5/OS5/HY4 categories.
- Approximately 300 Finnish and 400 wider-European staged contacts, across 11 non-Finnish countries.
- Recruitment sourcing channels and screening criteria.
- Approximate implementation windows from early October to 30 October 2026.
- Dataset freeze date of 30 October 2026.

The underlying pilot worksheets, named lead-list files, invitation dispatch logs and exact participant notice were not present in the repository snapshot reviewed. These details are therefore attributed to the researchers' records and are not described as independently audited. No response rate, exact invitation count, exact dispatch date or storage-control claim is inferred.

## External verification sources

1. Karelia University of Applied Sciences. Thesis Instructions: Starting Points. https://libguides.karelia.fi/thesis_instructions. Accessed 5 November 2026.
2. Karelia University of Applied Sciences. Report Outline. https://libguides.karelia.fi/c.php?g=689495&p=4935741. Accessed 5 November 2026.
3. Karelia University of Applied Sciences. Data Management Plan. https://libguides.karelia.fi/c.php?g=689495&p=5202279. Accessed 5 November 2026.
4. Karelia University of Applied Sciences. Use of AI in Karelia UAS Theses. https://libguides.karelia.fi/c.php?g=689495&p=5183606. Accessed 5 November 2026.
5. American Association for Public Opinion Research (AAPOR). Best Practices for Survey Research. https://aapor.org/standards-and-ethics/best-practices/. Accessed 5 November 2026.
6. European Data Protection Board (EDPB). Anonymisation / pseudonymisation. https://www.edpb.europa.eu/topics/ai-and-technology/anonymisation-pseudonymisation_en. Accessed 5 November 2026.
7. European Union. Regulation (EU) 2016/679 (General Data Protection Regulation), Article 5. https://eur-lex.europa.eu/eli/reg/2016/679/. Accessed 5 November 2026.
8. Tally. Conditional Logic. https://tally.so/help/conditional-form-logic. Accessed 5 November 2026.
9. Espino-Rodríguez, T. F. & Padrón-Robaina, V. 2006. A review of outsourcing from the resource-based view of the firm. International Journal of Management Reviews 8 (1), 49–70. https://doi.org/10.1111/j.1468-2370.2006.00120.x.
10. Hoecht, A. H. & Trott, P. 2006. Outsourcing, information leakage and the risk of losing technology based competencies. European Business Review 18 (5), 395–412. https://doi.org/10.1108/09555340610686967.
11. Lockamy, A. III & McCormack, K. 2010. Analysing risks in supply networks to facilitate outsourcing decisions. International Journal of Production Research 48 (2), 593–611. https://doi.org/10.1080/00207540903175152.
12. Williamson, O. E. 2008. Outsourcing: Transaction cost economics and supply chain management. Journal of Supply Chain Management 44 (2), 5–16. https://doi.org/10.1111/j.1745-493X.2008.00051.x.

## Remaining evidence required before submission

- The VGPS problem list and suggested-fix report should be placed in the repository or supplied in the conversation if it is intended to be the controlling audit checklist. It was not available in the accessible file search for this revision.
- Check the final participant information notice and data-management plan against Chapters 3 and 4.
- Retain the four pilot notes, both lead-list files and outreach dispatch logs in the project archive.
- Confirm with the supervisor whether a research permit or ethical review was required and document the decision and any approval or permission obtained.
- Check the Karelia UAS thesis template, citation format and AI-use requirements at final formatting stage.
