# GreenGut report card

GreenGut turns a poultry fecal qPCR panel (20 bacterial targets plus total bacteria) into a three-page gut health report card, comparing each bacterium with healthy chicks aged 0 to 21 days.

- `index.html`: report card with the reference built from compiled per-run values (NCBI SRA STAT classification), 228 chicks.
- `fastq.html`: the same report card with the reference rebuilt from raw FASTQ reads (DADA2 1.38, SILVA 138.2), 63 chicks.
- `example_excel_reference.csv`, `example_fastq_reference.csv`: example upload files with three flocks each.

Everything runs in the browser. Uploaded files are not sent anywhere.

Status: research prototype. The reference population is built from public datasets and is pending prospective field validation. The report describes a sample; it does not diagnose disease.
