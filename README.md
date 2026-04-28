# DeepSemantics: Multilingual Polarization Detection (SemEval-2026)

This repository contains the winning architecture for fine-grained polarization detection in English and Hausa social media posts, developed for **SemEval-2026 Task 9 (POLAR)**.

## 🚀 Research Impact
Our system ranked **6th globally on the Hausa track** and **15th on the English track**. We address the challenge of identifying polarization manifestations (Vilification, Dehumanization, Extreme Language) in low-resource and multilingual settings.

## 🛠 Model Architecture
The core architecture implements a **One-vs-Rest (OvR) framework** utilizing:
- **Encoders:** RoBERTa (English) and Afro-XLM-R (Multilingual/Hausa).
- **Loss Function:** Adaptive Focal Loss to handle severe class imbalance in social media datasets.
- **Optimization:** Per-label threshold optimization for maximized Macro-F1 performance.

## 📊 Results
| Language | Metric (Macro-F1) | Global Rank |
|----------|-------------------|-------------|
| English  | 0.464             | 15th        |
| Hausa    | 0.192             | 6th         |

## 📓 Notebook Structure
1. Subsract_1_final.ipynb: Data preprocessing and XLM-R tokenization pipelines.
2. substack_2_final.ipynb: Model training and Adaptive Focal Loss implementation.
3. substack_3_final.ipynb: Threshold optimization and final ensemble strategy.

## ⚙️ Requirements
- PyTorch
- HuggingFace Transformers
- Scikit-learn
- Pandas/NumPy

## 🎓 Author
**Eliasse TIAO** — Google DeepMind Scholar | M.Sc. AI Student @ AIMS.
