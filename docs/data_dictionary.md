# Data Dictionary

This file describes the main workbook supplied in `data/vit_medical_imaging_slr_worksheet.xlsx`.

## Workbook overview

| Sheet | Purpose | Approximate scope |
|---|---|---|
| `Title & PRISMA` | Space reserved for title/PRISMA-level summary information. | Repository metadata / PRISMA summary support. |
| `Databases & Years` | Database-year level source information used to support the review search summary. | Search-source summary. |
| `All_Extracted` | Raw extracted records before deduplication/screening. | 683 records. |
| `Deduplicated` | Records after duplicate removal. | 482 records. |
| `Screened` | Title/abstract/keyword screening decisions and criteria. | 482 screened records. |
| `Eligibility` | Full-text eligibility and quality-assessment data. | 297 records assessed. |
| `Included` | Final included studies with bibliographic details and extracted summaries. | 109 included studies. |
| `Master Table` | Main coded extraction table used for the RQ-level synthesis. | 109 included papers, 61 fields. |

## Key worksheet fields

The exact columns differ by sheet, but the main recurring fields are listed below.

### Bibliographic identity fields

- `Name of Database` / `Source Database`: Database from which the record was retrieved.
- `Reference Type` / `Publication Type`: Journal article, conference paper, or other publication type.
- `Author` / `Authors`: Author names as recorded in the source export or coded extraction.
- `Year`: Publication year.
- `Title`: Full publication title.
- `Journal` / `Journal / Conference`: Publication venue.
- `Publisher`: Publisher when available.
- `DOI`: Digital Object Identifier when available.
- `URL`: Source URL when available.

### Screening and eligibility fields

- `Screening Decision`: Inclusion/exclusion decision during screening.
- `Criteria Met`: Inclusion criteria met at screening stage.
- `Objectives`, `Methodology`, `Limitations`, `Findings`: Eligibility and quality-assessment scoring categories.
- `Total` / `Quality Score`: Total quality-related score fields used during eligibility assessment.

### Master extraction fields

The `Master Table` groups fields into manuscript RQs:

- **Identity:** paper ID, title, authors, year, publication type, venue, DOI, source database, country.
- **RQ1 — Landscape:** imaging modality, target disease, clinical task, architecture family, model variant.
- **RQ2 — Architecture & Performance:** patch size, input dimensionality, attention mechanism, primary metric, accuracy, AUC, Dice, F1, sensitivity/recall, specificity, CNN comparison, ablation, statistical significance, external/multi-site validation.
- **RQ3 — Training & Data Efficiency:** pre-training strategy, pre-training dataset, transfer learning, self-supervision, augmentation, training-size category, dataset names, dataset availability, dataset size, class count, imbalance handling, multi-centre data.
- **RQ4 — Interpretability & Clinical Trust:** XAI method, XAI contribution, clinical decision-support framing.
- **RQ5 — Methodological Gaps:** limitation categories, future work, parameter count, inference time, hardware, code availability, data availability.

## Notes for users

- Empty cells generally mean that information was not reported or was not available in the source record.
- Percentages and metrics are reported as extracted from the corresponding publications where available.
- The worksheet is intended as a transparent audit trail for the systematic review rather than as a re-analysis script.
