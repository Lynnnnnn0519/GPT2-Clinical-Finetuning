🧠 GPT-2 Clinical Fine-Tuning on MIMIC-III

A domain adaptation experiment for clinical text generation

📌 Overview

This project fine-tunes GPT-2 on clinical notes from the MIMIC-III database to improve its ability to understand and generate medical text.
The goal is to perform domain adaptation and compare the performance of the base GPT-2 model with the fine-tuned version using:

Quantitative evaluation (Perplexity)

Qualitative evaluation (Generation comparison)

🗂 Dataset

Source: MIMIC-III NOTEEVENTS

Extracted fields: cleaned clinical notes

Sample size used: 20,000 notes

Dataset size: ~34 MB

🧪 Methods

Tokenization using HuggingFace GPT-2 tokenizer

Train/validation/test split: 80 / 10 / 10

Fine-tuning GPT-2 for 2 epochs

Evaluation using:

Perplexity on test set

Side-by-side text generation

📊 Results
Model	Perplexity
Base GPT-2	183.90
Fine-tuned GPT-2	8.29

The fine-tuned model produces significantly more realistic and clinically plausible text compared to the base GPT-2.
📁 Files

GPT2_Clinical_Finetuning.ipynb — full training + evaluation pipeline

README (this file)
