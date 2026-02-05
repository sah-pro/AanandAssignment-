Forced Alignment with Montreal Forced Aligner

This repository contains the outputs and supporting files for the forced alignment assignment from IIIT Hyderabad.

Contents

 `Assignment_outputs.zip` – contains the corpus and generated TextGrid files.
 `report.pdf` – documentation and observations.

How to Reproduce

1. Install Montreal Forced Aligner (MFA).
2. Place audio (`*.wav`) and transcripts (`*.txt`) under a folder named `corpus`.
3. Use the English acoustic model and dictionary:


mfa model download acoustic english_mfa
mfa model download dictionary english_us_arpa

4. Run validation:


mfa validate corpus english_us_arpa english_mfa

5. Run alignment:


mfa align corpus english_us_arpa english_mfa output

6. Aligned TextGrid files will be in `output/`.

## Notes

- The large files are stored in the ZIP due to size constraints.
- Extract to see the folder structure.
