# docs/

Source materials and references the skills are based on.

**These files are git-ignored** because the standards are copyrighted and shouldn't be redistributed via this public repo. The skills under `../skills/` paraphrase the rules; the source PDFs stay local.

## What lives here

Place these in this folder on each machine that needs them (they will be ignored by git):

### ANZSMM (measurement)
- `ANZSMM_4P_3.1.pdf` — Australian and New Zealand Standard Method of Measurement of Building Works, 2018 Edition. Published by AIQS, NZIQS, MBA Limited, RMBA NZ. ISBN 978-0-9599641-0-3.
- `ANZSMM_4P_3.1.txt` — Plain-text extract.

### ACMM (cost management)
- `ACMM_Vol1.pdf` — Australian Cost Management Manual, Volume 1 (Cost Management Process), Second Edition, June 2000 (reprint December 2015). Published by AIQS. ISBN 1-876389-06-0.
- `ACMM_Vol2.pdf` — Australian Cost Management Manual, Volume 2 (Sub-element Definitions and Method of Measurement), October 2001. ISBN 1-976389-10-9.
- `ACMM_Vol3.pdf` — Australian Cost Management Manual, Volume 3 (Life Cycle Costing). Published by AIQS.
- `ACMM_Vol1.txt`, `ACMM_Vol2.txt`, `ACMM_Vol3.txt` — Plain-text extracts.

## Where to get the official copies

- Australia: Australian Institute of Quantity Surveyors (AIQS) — https://www.aiqs.com.au
- New Zealand: New Zealand Institute of Quantity Surveyors (NZIQS) — https://www.nziqs.co.nz

## Generating the text extract

If you have `pdftotext` (bundled with Git for Windows under `C:\Program Files\Git\mingw64\bin\` on Windows), run:

```powershell
$pdftotext = "C:\Program Files\Git\mingw64\bin\pdftotext.exe"
& $pdftotext -layout ".\ANZSMM_4P_3.1.pdf" ".\ANZSMM_4P_3.1.txt"
& $pdftotext -layout ".\ACMM_Vol1.pdf" ".\ACMM_Vol1.txt"
& $pdftotext -layout ".\ACMM_Vol2.pdf" ".\ACMM_Vol2.txt"
& $pdftotext -layout ".\ACMM_Vol3.pdf" ".\ACMM_Vol3.txt"
```

```bash
pdftotext -layout ANZSMM_4P_3.1.pdf ANZSMM_4P_3.1.txt
pdftotext -layout ACMM_Vol1.pdf ACMM_Vol1.txt
pdftotext -layout ACMM_Vol2.pdf ACMM_Vol2.txt
pdftotext -layout ACMM_Vol3.pdf ACMM_Vol3.txt
```
