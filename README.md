# Vision Transformers in Medical Imaging — Systematic Review Repository

This repository contains the supplementary worksheet and supporting documentation for the manuscript:

**Vision Transformers in Medical Imaging: A Systematic Literature Review of Architectures, Training Strategies, Explainability, and Research Gaps**

The repository is intended to support transparency, reproducibility, and reviewer access to the screening log, eligibility and quality-assessment scores, included-study records, and master data-extraction table used in the review.

## Repository contents

| Path | Description |
|---|---|
| `data/vit_medical_imaging_slr_worksheet.xlsx` | Main worksheet containing the search, screening, eligibility/QEA, included-study, and master extraction data. |
| `docs/data_dictionary.md` | Description of each worksheet tab and the main data fields. |
| `docs/screening_protocol.md` | Summary of the search, screening, eligibility, and quality-assessment procedure. |
| `docs/data_availability_statement.md` | Repository-ready data availability wording that can be pasted into the manuscript after the GitHub link is created. |
| `docs/github_upload_steps.md` | Simple steps to upload this folder as a GitHub repository and obtain the repository link. |
| `metadata/paper_metadata.json` | Machine-readable manuscript and repository metadata. |
| `metadata/checksums_sha256.txt` | SHA-256 checksums for repository files. |
| `scripts/verify_repository.py` | Optional script to verify that required files are present and report checksums. |
| `CITATION.cff` | Citation metadata for GitHub and Zenodo. |
| `LICENSE` | CC BY 4.0 license text for reuse with attribution. |

## Data summary

The worksheet documents the systematic literature review process reported in the manuscript:

- Initial records: **683**
- Deduplicated/screened records: **482**
- Eligibility/QEA records: **297**
- Included studies: **109**
- Master extraction table: **109 included papers** with **61 recorded columns** across identity, RQ1 landscape, RQ2 architecture/performance, RQ3 training/data efficiency, RQ4 interpretability/clinical trust, and RQ5 methodological gaps.

## Main worksheet tabs

The Excel workbook includes the following tabs:

1. `Title & PRISMA`
2. `Databases & Years`
3. `All_Extracted`
4. `Deduplicated`
5. `Screened`
6. `Eligibility`
7. `Included`
8. `Master Table`

See [`docs/data_dictionary.md`](docs/data_dictionary.md) for details.

## How to use

1. Download or clone the repository.
2. Open `data/vit_medical_imaging_slr_worksheet.xlsx` in Microsoft Excel, LibreOffice Calc, or another spreadsheet tool.
3. Use the `Screened`, `Eligibility`, `Included`, and `Master Table` tabs to verify the PRISMA screening process and extracted evidence.
4. Use the metadata and checksum files to confirm that the repository contents have not changed after release.

## Suggested manuscript data availability statement

After uploading this repository to GitHub, update the placeholder URL below:

> The complete screening log, eligibility and quality-assessment scoresheet, included-study records, and master data-extraction table supporting this systematic review are available at: `https://github.com/<your-username>/<repo-name>`.

A longer version is provided in [`docs/data_availability_statement.md`](docs/data_availability_statement.md).

## Citation

Please cite the associated article when using this repository. A repository citation template is provided in [`CITATION.cff`](CITATION.cff).

## License

This repository is released under the Creative Commons Attribution 4.0 International License (CC BY 4.0). This allows reuse with appropriate attribution. Change the license before release if your journal, institution, or co-authors require a different license.
