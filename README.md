# Medical Named Entity Recognition (NER) Annotation Project

## Overview
This project demonstrates a rigorous, human-in-the-loop data annotation workflow for clinical text. Using a sample of de-identified clinical notes, I developed strict annotation guidelines and structured the unstructured medical data to train Large Language Models (LLMs) in extracting critical patient information.

## Objective
To accurately identify and classify key medical entities within raw clinical narratives to support automated telehealth documentation and chronic care monitoring.

## Methodology
1. **Data Sourcing:** Utilized a sample of publicly available, de-identified clinical text (mimicking the MIMIC-III database format).
2. **Guideline Development:** Authored comprehensive annotation rules for handling overlapping entities and clinical abbreviations.
3. **Manual Annotation:** Labeled text using character-level offset structures standard in NLP frameworks (e.g., spaCy, HuggingFace).
4. **Quality Assurance:** Documented edge cases and inter-annotator conflict resolutions to ensure high data fidelity.

## Repository Contents
* `Annotation_Guidelines.md`: The rulebook defining entity categories and edge-case handling.
* `sample_annotations.json`: The final structured dataset ready for machine learning ingestion.
* `QA_Log.md`: Documentation of ambiguous clinical phrasing and how it was resolved.
