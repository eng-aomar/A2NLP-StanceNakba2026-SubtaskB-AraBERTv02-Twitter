# 🏛️ A2NLP at StanceNakba 2026 (Subtask B)
### Fine-Tuned AraBERT for Topic-Based Arabic Stance Detection

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Space-blue)](https://huggingface.co/spaces/aomar85/A2NLP-StanceNakba2026)
[![License](https://img.shields.io/badge/License-Apache%202.0-green.svg)](https://opensource.org/licenses/Apache-2.0)

This repository contains the official implementation for the **A2NLP** system submitted to the **StanceNakba 2026 Shared Task (Subtask B)**. The work was presented at the **15th International Conference on Language Resources and Evaluation (LREC’26)** in Palma, Spain.

---

## 📝 Project Description
The **A2NLP-StanceNakba2026-SubtaskB-AraBERTv02-Twitter** system is designed to detect stances in Arabic social media discourse. By utilizing a prompt-based fine-tuning approach on **AraBERTv02**, the model identifies whether a text is **Pro (مؤيد)**, **Against (معارض)**, or **Neutral (محايد)** toward specific socio-political targets.

### Technical Highlights:
* **Architecture:** `aubmindlab/bert-base-arabertv02` with a sequence classification head.
* **Input Strategy:** Topic-conditioned prompts using the format:  
    `الهدف: [TOPIC] [SEP] الموقف من: [SENTENCE]`
* **Performance:** Achieved a **Validation Macro-F1 of 0.8434**.
* **Target Domain:** Dialectal Arabic (Levantine, Gulf, and Egyptian) as found on Twitter/X.

---

## 🚀 Getting Started

### 1. Installation
Clone the repository and install the necessary dependencies:
```bash
git clone [https://github.com/YourUsername/A2NLP-StanceNakba2026-SubtaskB-AraBERTv02-Twitter.git](https://github.com/YourUsername/A2NLP-StanceNakba2026-SubtaskB-AraBERTv02-Twitter.git)
cd A2NLP-StanceNakba2026-SubtaskB-AraBERTv02-Twitter
pip install -r requirements.txt
