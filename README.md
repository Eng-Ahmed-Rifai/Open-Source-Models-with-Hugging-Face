# 🤗 Open Source Models with Hugging Face — Foundation & Multimodal Pipelines

[![Hugging Face](https://img.shields.io/badge/Hugging_Face-Transformers-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)](https://huggingface.co/)
[![DeepLearning.AI](https://img.shields.io/badge/DeepLearning.AI-100%25_Verified-FF6F00?style=for-the-badge&logo=deeplearning)](https://www.deeplearning.ai/)
[![Live Simulator](https://img.shields.io/badge/Live_Simulator-Web_Demo-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://eng-ahmed-rifai.github.io/AI-Engineering-Interactive-Portfolio/)
[![License: MIT](https://img.shields.io/badge/License-MIT-34A853.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

> **Architect & Engineer:** [Eng. Ahmed Rifai](https://github.com/Eng-Ahmed-Rifai)  
> **Credential:** DeepLearning.AI & Coursera (Completed at 100.00% Grade Perfection)  
> **Master Portfolio:** [AI-Engineering-Interactive-Portfolio](https://github.com/Eng-Ahmed-Rifai/AI-Engineering-Interactive-Portfolio)  
> **Live Web Demo:** [Interactive Simulator](https://eng-ahmed-rifai.github.io/AI-Engineering-Interactive-Portfolio/)

---

## 📖 Curriculum Overview & Engineering Objectives

This repository contains production code implementations, architectural designs, and benchmarks developed throughout the **DeepLearning.AI Open Source Models with Hugging Face** curriculum.

The project demonstrates leveraging open-weights models hosted on the Hugging Face Hub across multimodal modalities (Natural Language Processing, Audio Transcription, Vision-Language understanding) without data privacy leakage or proprietary API dependencies.

### 🌟 Key Pipeline Patterns
1. **Multimodal Task Execution:**
   - Text Summarization: `facebook/bart-large-cnn` for executive document compression.
   - Zero-Shot Classification: `valhalla/distilbart-mnli-12-3` for arbitrary category labeling.
   - Speech Recognition (ASR): `openai/whisper-small` for multilingual transcription.
2. **Quantization & Efficiency (bitsandbytes):**
   - 8-bit and 4-bit NormalFloat (NF4) quantization reducing VRAM footprint by up to 75% for edge and local GPU deployment.
3. **Packaging & Deployment:**
   - Gradio application microservices deployed seamlessly to Hugging Face Spaces.

---

## 🏗️ Model Selection & Latency Matrix

| Task Modality | Benchmark Model | Parameters | Quantization Profile | Recommended Runtime |
|---|---|:---:|:---:|:---:|
| Abstractive Summarization | `facebook/bart-large-cnn` | 406M | FP16 / INT8 | GPU / Edge Cloud |
| Zero-Shot NLI Classification | `distilbart-mnli-12-3` | 231M | FP16 / CPU-Quantized | Standard CPU |
| Multilingual Speech (ASR) | `openai/whisper-small` | 244M | INT8 via bitsandbytes | Edge / Cloud Run |

---

## 📂 Repository Structure

```
.
├── README.md               # Complete architectural documentation & benchmarks
├── multimodal_pipeline.py  # Production multi-task pipeline hub implementation
├── demo_hf_models.py       # Interactive CLI runner
├── requirements.txt        # Python dependencies
└── LICENSE                 # MIT License
```

---

## 🚀 Quick Start & Execution

```bash
# Clone the repository
git clone https://github.com/Eng-Ahmed-Rifai/Open-Source-Models-with-Hugging-Face.git
cd Open-Source-Models-with-Hugging-Face

# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run CLI demonstration
python demo_hf_models.py
```

---

## 📜 Verified Coursera & DeepLearning.AI Credential
- **Course:** Open Source Models with Hugging Face (DeepLearning.AI)
- **Learner:** Eng. Ahmed Rifai
- **Completion Date:** October 21, 2026
- **Grade Achieved:** **100.00%** (All graded items passed at 100%)

---

## 📄 License & Attribution
Licensed under the [MIT License](LICENSE).  
*Built with AI Agent assistance.*
