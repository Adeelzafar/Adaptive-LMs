# How to use Language Models for Vehicle Service Complaint Classification under Industrial Constraints?

This repository contains the code and experimental setup for our empirical study on adapting Large Language Models (LLMs) and Small Language Models (SLMs) to classify vehicle service complaints under industrial constraints.

## 📌 Project Overview
In industrial settings, classifying service reports is challenged by noisy data, multilingual inputs, and limited annotation budgets. This project evaluates two primary adaptation strategies:
1. **Structured Prompting:** Using Small Language Models (SmolLM2, Llama-3.2) with rich metadata.
2. **Supervised Fine-Tuning (SFT):** Using BERT, including a "Public-to-Private" transfer learning strategy.

### Key Findings
* **The "Cold-Start" Strategy:** Fine-tuning BERT on a large public dataset (NHTSA) before adapting to proprietary data improves F1-score from **0.57 to 0.92**.
* **Metadata Importance:** Incorporating structured metadata into SLM prompts is critical; removing it causes a performance drop from **0.92 to 0.40**.
* **Model Efficiency:** 1-2B parameter models (SmolLM2) achieve performance comparable to larger fine-tuned models when structured prompting is used.

---

