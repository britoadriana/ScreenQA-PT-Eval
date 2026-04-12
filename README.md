# 📱 ScreenQA-PT: VLM Analysis & UX Metrics

[![Hugging Face Dataset](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Dataset-yellow)](https://huggingface.co/datasets/britoadriana/screen_qa_portuguese)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)

This repository contains the official implementation and evaluation scripts for **ScreenQA-PT**, a Portuguese-language benchmark for User Interface Question Answering (ScreenQA). 

Our research **introduces ScreenQA-PT** and provides a comprehensive comparative analysis against the original **ScreenQA** dataset. We explore the capabilities of state-of-the-art **Vision Language Models (VLMs)** in understanding mobile layouts and answering UX-related questions across different languages.

---

## 🔍 Research Overview

| Category | Details |
| :--- | :--- |
| **Datasets** | **ScreenQA-PT** (Our Portuguese benchmark) & **ScreenQA** (Original English version) |
| **Models** | Extensive evaluation using multiple VLMs (e.g., Qwen2.5-VL and others) |
| **Lexical Metrics** | SQuAD F1 and Exact Match (EM) |
| **Semantic Metrics** | Multilingual Cosine Similarity via Sentence Embeddings |
| **Structural Metrics** | Screen complexity analysis |

---

## 🛠 Implementation Details

To ensure clarity and reproducibility of the results presented in our paper, we have organized the source code as follows:

* **🚀 Representative Examples:** Instead of providing redundant scripts for every experiment, we provide high-quality, streamlined examples for each stage of the pipeline: **Classification, Inference, and Evaluation**. The same logic was applied across all VLMs and datasets mentioned in the study.
* **🌍 English Standardization:** All variables, function names, and comments have been translated into English to facilitate understanding for the global AI and UX research community.
* **🧹 Production-Ready Cleaning:** Notebooks were refactored to remove debugging logs and redundant steps, focusing on the core logic used to generate the final metrics.

---

## 📁 Repository Structure

```text
├── notebooks/
│   ├── screen_complexity_analysis.ipynb   # Image density and fragmentation
│   ├── question_classification.ipynb      # VLM taxonomy classification
│   └── inference_and_evaluation.ipynb     # Main evaluation pipeline
├── requirements.txt                       # Necessary libraries
└── README.md                              # Project documentation
