# Greek Medical Speech Transcription System

This repository contains code, models, and evaluation results from a thesis project focused on building a domain-specific **Automatic Speech Recognition (ASR) system for Greek medical dictation**. The system combines fine-tuned Whisper models with a Greek GPT-2 language model for re-ranking, aiming to improve transcription accuracy for medical documentation.

---

## Repository Structure

- **Code**: Jupyter notebooks for model fine-tuning.
  - `Finetuning_Whisper.ipynb` – Fine-tuning Whisper models on Greek medical speech data.
  - `greek-gpt2.ipynb` – Fine-tuning GPT-2 for Greek medical text.
  
- **Data**: Dataset exploration and sample data.
  - `datasets-samples.ipynb` – Overview of the datasets used for training and evaluation.
  
- **Evaluation**: Model and pipeline performance analysis.
  - `models-evaluation.ipynb` – Evaluation of individual models (Whisper and GPT-2).
  - `pipeline-evaluation.ipynb` – Evaluation of the full Whisper + GPT-2 pipeline.
  
- **Models**: Documentation for each trained model.
  - `Greek-Medical-GPT2.txt`
  - `Whisper-Large-Greek.txt`
  - `Whisper-Medium-Greek.txt`
  - `Whisper-Small-Greek.txt`
  - `greek-mT5-medical.txt`

---

## Project Overview

Accurate Greek medical transcription is a challenging and under-resourced task. Traditional ASR systems perform poorly due to:

- Complex medical terminology.
- Greek-specific linguistic patterns.
- Variations in speech (dialects, accents, noise).

This project develops a **Whisper-GPT-2 pipeline**:

1. **Whisper ASR** generates multiple transcription hypotheses (Small, Medium, Large models).
2. **Greek GPT-2** re-ranks these hypotheses based on grammatical correctness, contextual relevance, and semantic coherence.
3. The best candidate is selected as the final transcription.

This approach integrates **acoustic and linguistic modeling** to handle domain-specific terminology and improve transcription accuracy.

---

