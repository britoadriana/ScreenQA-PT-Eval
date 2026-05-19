# 📱 ScreenQA-PT: Multicriteria Auditing Framework for Mobile UI Understanding

[![Hugging Face Dataset](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Dataset-yellow)](https://huggingface.co/datasets/britoadriana/screen_qa_portuguese)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)

**Portuguese Diagnostic Benchmark for Reliability Auditing in Vision-Language Models**
Hugging Face Dataset • MIT License • Python 3.10+

This repository contains the official implementation and evaluation pipeline for **ScreenQA-PT**, a manually curated Portuguese evaluation suite designed for **auditing semantic reliability in Vision-Language Models (VLMs)** applied to mobile User Interface Understanding.

Rather than focusing exclusively on benchmark ranking, this project investigates how multimodal systems behave under **cross-lingual**, **uncertainty-sensitive**, and **localized UI interpretation** conditions.

The repository accompanies our research on **multicriteria reliability auditing** for VLM-based UI understanding systems.

---

# 🔍 Research Focus

Current benchmark accuracy often overestimates the reliability of multimodal systems in realistic interface interpretation scenarios.

This project investigates critical failure modes such as:

* semantic misinterpretation,
* failures to abstain in unanswerable cases,
* cross-lingual degradation,
* disagreement between lexical and semantic evaluation metrics.

To support this analysis, we propose a **multicriteria auditing framework** combining lexical, semantic, and judgment-based evaluation criteria.

---

# 🧠 Auditing Dimensions

| Auditing Dimension      | Description                                                 |
| ----------------------- | ----------------------------------------------------------- |
| Semantic Reliability    | Whether the model preserves the intended semantic meaning   |
| Abstention Robustness   | Ability to appropriately handle unanswerable questions      |
| Cross-Lingual Stability | Performance degradation across English and Portuguese       |
| Metric Agreement        | Divergence between lexical and semantic evaluation criteria |
| Verbosity Sensitivity   | Impact of response length on evaluation metrics             |

---

# 📊 Evaluation Framework

## Datasets

* **ScreenQA-PT** — manually curated Portuguese diagnostic evaluation suite
* **ScreenQA** — original English benchmark

## Evaluated Models

* Qwen2.5-VL
* LLaVA-v1.6
* Llama-4-Maverick
* Additional VLMs can be integrated into the evaluation pipeline

## Evaluation Criteria

### Lexical Metrics

* SQuAD Exact Match (EM)
* SQuAD F1

### Semantic Metrics

* Multilingual cosine similarity via sentence embeddings
* LLM-as-a-judge semantic scoring

### Reliability Analysis

* No-answer failure analysis
* Cross-lingual robustness evaluation
* Metric disagreement analysis
* Verbosity correlation analysis

### Structural Screen Metrics

* Visual density
* UI fragmentation
* Interface complexity analysis

---

# 🎯 About ScreenQA-PT

ScreenQA-PT is **not intended as a large-scale benchmark replacement**.

Instead, it functions as a:

* localized stress-test dataset,
* diagnostic evaluation suite,
* manually curated auditing instrument

designed to expose reliability limitations in multimodal UI understanding systems under Portuguese-language and localized interface conditions.

The dataset prioritizes:

* semantic consistency,
* annotation quality,
* localization realism,
* uncertainty-sensitive evaluation.

---

# 🛠 Repository Design Principles

To improve reproducibility and facilitate auditing-oriented experimentation, the repository follows a streamlined and modular structure.

## Key Design Choices

### 🔬 Auditing-Oriented Evaluation

The repository emphasizes reliability inspection and failure analysis rather than leaderboard-style benchmarking.

### 🌍 Cross-Lingual Evaluation

All scripts support multilingual evaluation workflows for English and Portuguese UI understanding.

### 🧹 Research-to-Production Refactoring

Experimental notebooks were cleaned and standardized to expose only the final evaluation logic used in the study.

### 📦 Representative Pipelines

Instead of publishing redundant scripts for every experimental variation, we provide representative implementations for:

* inference,
* evaluation,
* task categorization,
* screen complexity analysis.

---

# 📁 Repository Structure

```text
├── notebooks/
│   ├── screen_complexity_analysis.ipynb
│   │   └── Visual density and UI fragmentation analysis
│   │
│   ├── task_classification.ipynb
│   │   └── Functional UX task categorization pipeline
│   │
│   ├── inference_pipeline.ipynb
│   │   └── VLM inference workflow for ScreenQA and ScreenQA-PT
│   │
│   ├── multicriteria_evaluation.ipynb
│   │   └── Lexical, semantic, and judge-based auditing metrics
│   │
│   └── reliability_analysis.ipynb
│       └── Cross-lingual robustness and failure-mode analysis
│
├── requirements.txt
├── LICENSE
└── README.md
```

---

# ⚠ Important Note

This repository focuses on **early-stage reliability auditing** of multimodal systems.

The proposed framework is intended to support:

* scalable semantic inspection,
* failure-mode identification,
* robustness analysis,
* cross-lingual evaluation.

It is **not intended to replace human-centered evaluation** when claims involve:

* usability,
* trust,
* interaction quality,
* user experience.

---

# 📚 Citation

```bibtex
@article{screenqapt2026,
  title={A Multicriteria Auditing Framework for Mobile UI Understanding in Vision-Language Models},
  author={Anonymous Authors},
  year={2026}
}
```

---

## 📁 Repository Structure

```text
├── notebooks/
│   ├── screen_complexity_analysis.ipynb   # Image density and fragmentation
│   ├── question_classification.ipynb      # VLM taxonomy classification
│   └── inference_and_evaluation.ipynb     # Main evaluation pipeline
├── requirements.txt                       # Necessary libraries
└── README.md                              # Project documentation
