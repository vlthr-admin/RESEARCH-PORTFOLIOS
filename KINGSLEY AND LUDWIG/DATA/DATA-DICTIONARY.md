# Data Dictionary — Readable Response Dataset

Source: `DATA/responses.csv` (unchanged). Analysis copy: `DATA/responses-readable.csv`.  
Current snapshot: 30 respondent records, 29 fields. The questionnaire did not collect verified organisation IDs; do not describe these as 30 unique companies.

| Source field | Readable field | Definition |
|---|---|---|
| `profile_id` | Respondent Record ID | Sequential row identifier; not a respondent name or verified organisation identifier. |
| `country` | Country | Country reported by respondent. |
| `industry` | Industry | Industry reported by respondent. |
| `role_function` | Respondent Role or Function | Respondent's role/function. |
| `knowledge_level` | Level of Operational Knowledge | Self-reported familiarity/responsibility for assessed activity. |
| `company_size` | Company Size (Employees) | Reported employee-size band. |
| `activity` | Activity Assessed | Specific company activity assessed; unit of analysis. |
| `operating_model` | Operating Model | Operating model used for assessed activity; primary grouping variable. |
| `internal_skill_dependency` | Dependence on Internal Skills (1–10) | In-house branch rating; dependence on internal skills. |
| `internal_control_effectiveness` | Effectiveness of Internal Control (1–10) | In-house branch rating; effectiveness of internal control. |
| `internal_resource_disruption` | Impact of Internal Resource Disruption (1–10) | In-house branch rating; impact if internal resources are unavailable. |
| `internal_scalability` | Ease of Internal Scaling (1–5) | In-house branch rating; ease of scaling internal capacity. |
| `primary_inhouse_risk` | Primary In-House Risk | Primary risk selected for in-house activity. |
| `supplier_dependency` | Dependence on External Supplier (1–10) | Outsourced branch rating; dependence on supplier/provider. |
| `supplier_monitoring_effectiveness` | Effectiveness of Supplier Monitoring (1–10) | Outsourced branch rating; effectiveness of supplier monitoring. |
| `supplier_disruption` | Impact of Supplier Disruption (1–10) | Outsourced branch rating; impact of supplier disruption. |
| `provider_replacement_ease` | Ease of Replacing Provider (1–5) | Outsourced branch rating; ease of replacing provider. |
| `primary_outsourcing_risk` | Primary Outsourcing Risk | Primary risk selected for outsourced activity. |
| `responsibility_clarity` | Clarity of Responsibilities (1–10) | Hybrid branch rating; clarity of responsibilities. |
| `cross_boundary_information` | Effectiveness of Cross-Boundary Information (1–10) | Hybrid branch rating; cross-boundary information effectiveness. |
| `handoff_effectiveness` | Effectiveness of Operational Handoffs (1–10) | Hybrid branch rating; operational handoff effectiveness. |
| `primary_hybrid_risk` | Primary Hybrid-Model Risk | Primary risk selected for hybrid activity. |
| `problem_detection` | Effectiveness of Problem Detection (1–10) | Common rating; effectiveness of problem detection. |
| `recovery_effectiveness` | Effectiveness of Recovery (1–10) | Common rating; effectiveness of recovery. |
| `accountability_clarity` | Clarity of Accountability (1–10) | Common rating; clarity of accountability. |
| `failure_consequences` | Reported Failure Consequences (Multiple Selection) | Multi-select failure consequences; categories may overlap. |
| `make_buy_factors` | Make-or-Buy Decision Factors (Multiple Selection) | Multi-select make-or-buy factors; categories may overlap. |
| `overall_risk_effect` | Perceived Overall Risk Effect | Respondent perception of overall risk effect; not an objective risk measure. |
| `additional_insight` | Additional Insight (Optional) | Optional free text. Source entries all N/A; blank in analysis copy. |

## Branch applicability
- In-house branch: 9 applicable respondents.
- Outsourced branch: 12 applicable respondents.
- Hybrid branch: 9 applicable respondents.

Blank values in other branches are structurally not applicable under questionnaire routing. They are not imputed and are not counted as unanswered responses.

## Analysis rules
- Report applicable denominators for branch-specific measures.
- 1–5 and 1–10 scales are not directly comparable.
- Multi-select percentages may exceed 100% in total.
- Deduplicate respondents when harmonising Cost + Total cost as **Cost and financial considerations**, and Control + Direct control as **Control and operational authority**.
- Additional Insight is optional. All 30 source values are N/A; the analysis copy leaves these cells blank. No qualitative coding or quotations are supported.
- Only headers and the optional N/A placeholders were changed in the analysis copy. All other response values and row order are preserved.
