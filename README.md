# HEART-Synth

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.20214885.svg)](https://doi.org/10.5281/zenodo.20214885)


HEART-Synth is a synthetic resident-patient dialogue dataset for development-stage research on medical error disclosure assessment. The dataset contains synthetic multi-turn disclosure conversations with ordinal labels for five HEART domains:

- **H**: Hold Space and Stay Present  
- **E**: Explain the Facts  
- **A**: Apologize with Accountability  
- **R**: Relate with Empathy  
- **T**: Talk Through the Plan  

Each domain is scored from **0 to 3**. The dataset is intended for research on automated rubric-based assessment, synthetic clinical dialogue generation, dataset auditing, shortcut learning, and baseline model development.

## Dataset Description

The released dataset includes synthetic transcripts generated for resident-patient medical error disclosure scenarios. Each record contains:

- a unique `video_id`
- a multi-turn resident-patient transcript
- synthetic timestamp fields for possible future multimodal alignment
- HEART-domain scores and short score justifications

Audit-only metadata, such as scenario type, error type, patient profile, and intended performance profile, is separated from the main training input and should not be used as model input.

## Intended Use

This dataset is intended for:

- development and testing of automated scoring models
- analysis of rubric-based clinical communication assessment
- synthetic dataset auditing
- shortcut-learning and lexical-bias analysis
- preliminary model development before human-rated clinical data are available

HEART-Synth is **not** a clinical validation benchmark and should not be used for real clinical decision-making.

## Repository Contents

This repository include:

```text
HEART-Synth data/                  # HEART-Synth transcript JSON files
metadata.jsonl              # audit-only metadata
score_distribution.json              # Score distribution
README.md
```

## Citation

If you use HEART-Synth, please cite the archived dataset release:

Ghimire, A., Amsaad, F., & Adkins, S. (2026). HEART-Synth: A Synthetic Resident-Patient Dialogue Dataset for Medical Error Disclosure Assessment (v1.0.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.20214885

## Disclaimer

This dataset contains synthetically generated clinical communication transcripts created for research purposes. It does not contain real patient information or protected health information (PHI).




