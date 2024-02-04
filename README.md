# Data Centric Approach to SemEval-2024 Task 2

### Overview
This repository contains the code for the Data Centric Approach to SemEval-2024 [Task 2: Biomedical Natural Language Inference in Clinical Trials](https://sites.google.com/view/nli4ct/semeval-2024).

This project is conducted by Anna Barwig, Pingjun Hong and Shijia Zhou under the structure of the seminar Biomodical Natural Language Processing at LMU.

### Requirements
- Python
- PyTorch
- NumPy
- scikit-learn
- datasets
- transformers
- pandas
- wandb
- pickle

### Models
Please download the necessary pre-trained model from [huggingface](https://huggingface.co/)

DeBERTa-Base: [MoritzLaurer/DeBERTa-v3-base-mnli-fever-anli](https://huggingface.co/MoritzLaurer/DeBERTa-v3-base-mnli-fever-anli)

Flan-T5-Base: [google/flan-t5-base](https://huggingface.co/google/flan-t5-base)

### Evidence Retrieval Process
**Evidence Retrieval Documentations**

The evidence retrieval documentation are saved under the `evidence retrieval` repository:
- Evidence Retrieval for DeBERTa: `evidence_retrieval_DeBERTa.xlsx`
- Evidence Retrieval for Flan: `evidence_retrieval_Flan.xlsx`

**Annotators**

- DeBERTa instances: Anna Barwig, Pingjun Hong
- Flan instances: Pingjun Hong, Shijia Zhou

### Data Statements Generation
- Code for data selection: `data_selection_for_generation_round.ipynb`
- Statements generation: `data_statement_generation.xlsx`

### Results

The final predictions on test set are saved under the `predictions` repository:
- Predictions on test set of Flan: `predictions_Flan`
- Predictions on test set of DeBERTa (without classification boundary modification): `predictions_DeBERTa`
- Predictions on test set of DeBERTa (classification boundary modification 3:7): `predictions_DeBERTa_37`
- Predictions on test set of DeBERTa (classification boundary modification 4:6): `predictions_DeBERTa_46`

The corresponding scores are saved under the `results` repository:
- Results on test set of Flan: `scores_Flan`
- Results on test set of DeBERTa (without classification boundary modification): `scores_DeBERTa`
- Results on test set of DeBERTa (classification boundary modification 3:7): `scores_DeBERTa_37`
- Results on test set of DeBERTa (classification boundary modification 4:6): `scores_DeBERTa_46`
