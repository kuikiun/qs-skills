# docs/

Source materials and references the skills are based on.

**These files are git-ignored** because the standards are copyrighted and shouldn't be redistributed via this public repo. The skills under `../skills/` paraphrase the rules; the source PDFs stay local.

## What lives here

Place these in this folder on each machine that needs them (they will be ignored by git):

- `ANZSMM_4P_3.1.pdf` — Australian and New Zealand Standard Method of Measurement of Building Works, 2018 Edition. Published by AIQS, NZIQS, MBA Limited, RMBA NZ. ISBN 978-0-9599641-0-3.
- `ANZSMM_4P_3.1.txt` — Plain-text extract (produced by `pdftotext -layout`) for grep/search.

## Where to get the official copy

- Australia: Australian Institute of Quantity Surveyors (AIQS) — https://www.aiqs.com.au
- New Zealand: New Zealand Institute of Quantity Surveyors (NZIQS) — https://www.nziqs.co.nz

## Generating the text extract

If you have `pdftotext` (bundled with Git for Windows under `C:\Program Files\Git\mingw64\bin\` on Windows), run:

```powershell
& "C:\Program Files\Git\mingw64\bin\pdftotext.exe" -layout `
    ".\ANZSMM_4P_3.1.pdf" `
    ".\ANZSMM_4P_3.1.txt"
```

```bash
pdftotext -layout ANZSMM_4P_3.1.pdf ANZSMM_4P_3.1.txt
```
