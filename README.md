# Canine Cancer Research Project

**Collaborators:** Diya Saha, Jenny Lee, Kyuho Oh, Ian Raymond Domingo 
**Affiliation:** UC Irvine & Anivive Lifesciences


## Overview

This project focuses on automating the generation of patient summaries from clinical reports of canine cancer subjects. Traditionally, these summaries were manually written by veterinarians. By leveraging modern OCR and large language models (LLMs), we developed an end-to-end pipeline that extracts structured information from scanned clinical documents and generates accurate summaries in a scalable, automated manner.

## Objectives

* Extract structured data from unstructured clinical PDF reports using an OCR pipeline.
* Fine-tune named entity recognition (NER) models for biomedical and veterinary domains.
* Generate readable patient summaries using LLMs such as GPT, Claude, and LLaMA.
* Identify and analyze uncertain genetic variants and biomarkers.
* Provide a black-box, front-end interface to enable seamless adoption by clinical researchers.

## Key Contributions

* **OCR Integration:** Extracted relevant clinical features from PDF reports using a fine-tuned OCR model.
* **NER & Entity Analysis:** Leveraged SpaCy and GlinER for custom entity recognition on clinical language.
* **Summarization Pipeline:** Used large language models to generate structured patient overviews.
* **Uncertainty Analysis:** Extracted and tagged uncertain mutation variants for downstream analysis.
* **Tooling & Interface:** Designed a prototype interface for black-box deployment of the solution.

## Repository Structure

* `Extracting_DNA_summary.ipynb`: Extracts DNA-level features from reports.
* `Extracting_mutation_summaries.ipynb`: Summarizes mutation-related findings.
* `Generating_Overview.ipynb`: Uses LLMs to generate patient summaries.
* `NER_GlinerSpacy.ipynb`: Performs named entity recognition using SpaCy and GlinER.
* `NER_clndata.csv`, `NER_summ.csv`: Sample datasets used for NER tasks.
* `extracting_uncertainVariants.ipynb`: Identifies uncertain genetic variants.
* `tablular_to_llm.ipynb`: Transforms structured tabular data for LLM summarization.
* `Scoring_Evaluation.ipynb`: Evaluates the quality of generated summaries.
* `Problem_files.txt`: Logs files that encountered errors or incomplete parsing.

## Dependencies

* Python 3.x
* Jupyter Notebooks
* `pandas`, `numpy`, `matplotlib`
* `spacy`, `transformers`, `openai`, `llama-cpp`, etc.

## How to Use

1. Clone the repository.
2. Run `Extracting_DNA_summary.ipynb` and `Extracting_mutation_summaries.ipynb` to extract structured data.
3. Use `Generating_Overview.ipynb` to generate patient summaries.
4. Explore named entity recognition with `NER_GlinerSpacy.ipynb`.
5. Run `Scoring_Evaluation.ipynb` to evaluate generated outputs.

## License

This project is for academic and internal research purposes only.

---
