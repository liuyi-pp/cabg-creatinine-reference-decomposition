# CABG creatinine-reference decomposition

Code and selected aggregate review material for the r4 methods application, version aki-code-2026-11-17-rc7. Software creators: Yi Liu, Hui Wang, Qian Sun (confirmed order).

## Download and test

The complete portable source tree is inside **Additional_file_2_Code_and_aggregate_review_rc7.zip** in this repository. Download that fixed ZIP, check its SHA-256 against SHA256SUMS.txt and extract it. The original directory layout is preserved inside the ZIP; this repository root is a distribution wrapper rather than a flattened source tree.

From the extracted code root run with ordinary Python:

    python -X utf8 -B review_tools/check_release_bundle.py --report ../release_check.json

Use a new report path outside the snapshot. The checker uses only the standard library and validates code/manifest integrity and existing primary point/SMD/flow/denominator arithmetic. It does not execute clinical classification or reproduce clustered bootstrap confidence intervals. No simulated patient data are used. Authorized-source execution instructions and the historical R point-check workflow are included in the archive.

## Scope and licences

No patient-level records, complete retained formal outputs, hospital-specific fine cells or cluster-resampling inputs are distributed. Each analyst must independently obtain lawful source access to MIMIC-IV 3.1 and eICU-CRD 2.0. The article studies recorded creatinine-rise ascertainment, not a new clinically validated AKI definition.

MIT applies to original software; CC BY 4.0 applies to original documentation, figure-source material and selected shareable aggregates within LICENSE_SCOPE.md. Source-database and third-party rights are excluded. The representative confirmed release permission under the applicable source/institution/third-party conditions.

Independent external source-classification/CI reproduction has not been completed. Figure 2 adds direct labels to unchanged original estimates and CIs. Numerical secondary/hospital analyses are inventoried but not used to claim robustness. Historical local-status strings within retained metadata describe their reporting origin, not current accessibility.

Citation metadata are in CITATION.cff. Zenodo archive information will be added after its actual creation and verification. Do not infer a registered DOI or completed independent validation from preparation alone.
