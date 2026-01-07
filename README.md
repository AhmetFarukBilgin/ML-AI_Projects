# ML-AI_Projects
Custom ML and AI projects
## Project Description

This project implements an LLM-supervised translation system on Google Colab
for translating UCI technical and regulatory documents from English to Turkish.

A large language model (Gemini) is used as a **teacher model** to generate
high-quality, terminology-consistent translations. The system enforces
domain-specific glossary rules and legal modality constraints (e.g. “shall”,
“must”, “may”) to ensure regulatory accuracy.

The OpenAI / Gemini API key is securely configured via Colab environment
variables and is not included in the repository.

The generated teacher translations are exported as CSV files and are intended
to be used for downstream student model fine-tuning (e.g. MarianMT).
