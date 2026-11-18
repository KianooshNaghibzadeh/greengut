# GreenGut qPCR Gut Health Report

GreenGut turns a poultry fecal qPCR panel (20 bacterial targets/groups plus the universal 16S assay) into a three-page gut health report, comparing each target with healthy chickens aged 0 to 21 days.

- `index.html`: report with the reference built from compiled per-run values (NCBI SRA STAT classification), 228 chickens.
- `fastq.html`: the same report with the reference rebuilt from raw FASTQ reads (DADA2 1.38, SILVA 138.2), 63 chickens.
- `example_excel_reference.csv`, `example_fastq_reference.csv`: example upload files (four samples each, one failing lab QC).

Version 0.3.0 (2026-11-18): loads reported relative to universal 16S and never forced to 100%; percentiles from quantified values only (P10 to P90 main, P5 and P95 exploratory); a target is scored only with at least 30 quantified reference values; duplicate, efficiency and control checks; no score on QC failure; Salmonella and Campylobacter reported separately; generic Clostridium not scored; Target Panel Coverage and Standardized Panel Distance replace Shannon and Aitchison distance; version stamp in every PDF.

Everything runs in the browser. Uploaded files are not sent anywhere.

Status: prototype research reference. The baseline comes from public 16S sequencing data and is not yet calibrated against qPCR. The report describes a sample; it does not diagnose disease.
