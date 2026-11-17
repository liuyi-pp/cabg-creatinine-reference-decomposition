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


Citation metadata are in CITATION.cff. The fixed rc7 ZIP is publicly archived at Zenodo: https://doi.org/10.5281/zenodo.24297481 (record https://zenodo.org/records/24297481). The ZIP SHA-256 is 5fff3ba03ad23e05471ae2a359db56baae6954314333f0eab7653aca5a2693a2. Public code access and archiving do not establish independent external source-classification or confidence-interval reproduction.



## Local CI verification supplement

The later CI verification tools and selected aggregate audit records are published in [the CI verification release](https://github.com/liuyi-pp/cabg-creatinine-reference-decomposition/releases/tag/ci-audit-2026-11-17-r3) and archived at [Zenodo DOI 10.5281/zenodo.24309804](https://doi.org/10.5281/zenodo.24309804). Download the named `Additional_file_3_CI_verification.zip` asset together with its exact `Additional_file_2_Code_and_aggregates.zip` companion, `RELEASE_README.txt` and `SHA256SUMS.txt`. Both ZIPs match the current manuscript attachments byte for byte. The automatically generated release Source code ZIP/TAR is a repository wrapper and does not replace the named assets.

The original rc7 ZIP and DOI above remain unchanged. Its historical filenames and hash differ from the normalized companion required by the CI checker. Preparation-time status records inside the frozen CI attachment are historical; current availability is established by the published release and record. MIT and CC BY 4.0 apply within the included file-specific scopes. No patient records or restricted cluster/resampling inputs are distributed. Independent external source-data/CI reproduction remains incomplete; public code access and stored-record checks do not establish third-party verification.
