<div align="center">

# 🧠 AI-101: Machine Learning & NLP Portfolio

### End-to-End Supervised Learning, Multimodal Fraud Detection & Transformer Summarisation

[![Student](https://img.shields.io/badge/Student-Aliaan%20Shams-1e3a8a?style=for-the-badge&logo=github)](https://github.com/Aliaan-70177202)
[![Roll No](https://img.shields.io/badge/Roll%20No-70177202-0f766e?style=for-the-badge)](https://github.com/Aliaan-70177202/AI101-ML-Assignment-70177202)
[![Section](https://img.shields.io/badge/Section-C-7c3aed?style=for-the-badge)](#)
[![Course](https://img.shields.io/badge/Course-AI--101%20Machine%20Learning-b45309?style=for-the-badge)](#)

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.4+-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-CUDA%20T4-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/Hugging%20Face-T5--Small-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![LaTeX](https://img.shields.io/badge/Reports-IEEEtran%20LaTeX-008080?style=flat-square&logo=latex&logoColor=white)
![Status](https://img.shields.io/badge/Submission-Complete%20%26%20Verified-16a34a?style=flat-square)

</div>

> [!IMPORTANT]
> **Academic Integrity & Leakage-Free Design:** All preprocessing scalers, imputers, encoders, and TF-IDF vocabularies across Tasks **A1**, **B1**, and **C2** are fitted strictly on training splits (`random_state=42`). Every experiment is documented with reproducible notebooks, high-resolution diagnostic plots, and 2-page IEEE conference reports.

---

## 📋 Student & Course Information

| Attribute | Details |
| :--- | :--- |
| **Student Name** | **Aliaan Shams** |
| **Roll Number** | `70177202` |
| **Class & Section** | BS Intelligent Systems — **Section C** |
| **Department & University** | Department of Intelligent Systems, **The University of Lahore (UOL)** |
| **Course** | **AI-101** — Machine Learning |
| **Course Instructor** | **Dr. Muhammad Awais**, AI Architect |
| **Selected Tasks** | **A1** (Tabular Classification) • **B1** (Multimodal Text + Tabular) • **C2** (Seq2Seq Transformer NLP) |
| **Governance & Dependencies** | [📜 AI Use Disclosure](AI_DISCLOSURE.md) • [📦 requirements.txt](requirements.txt) |

---

## 🗂️ Deliverables & Direct File Access

Click any link below to inspect the executed Jupyter notebooks, 2-page IEEE PDF reports, LaTeX source code, or diagnostic figures directly on GitHub:

| Task | Domain & Problem | Code Notebook | 2-Page IEEE PDF | LaTeX Source | Diagnostic Figures |
| :---: | :--- | :---: | :---: | :---: | :---: |
| **A1** | **Breast Cancer Diagnosis**<br>*(Clinical Binary Classification)* | [📓 `A1_notebook.ipynb`](A1_Breast_Cancer/A1_notebook.ipynb) | [📄 `70177202_A1_Report.pdf`](A1_Breast_Cancer/report/70177202_A1_Report.pdf) | [📝 `main.tex`](A1_Breast_Cancer/report/source/main.tex) | [📊 EDA](A1_Breast_Cancer/figures/a1_eda.png) • [📈 Results](A1_Breast_Cancer/figures/a1_results.png) |
| **B1** | **Fake Job Posting Detection**<br>*(Imbalanced Multimodal NLP + Tabular)* | [📓 `B1_notebook.ipynb`](B1_Fake_Job_Postings/B1_notebook.ipynb) | [📄 `70177202_B1_Report.pdf`](B1_Fake_Job_Postings/report/70177202_B1_Report.pdf) | [📝 `main.tex`](B1_Fake_Job_Postings/report/source/main.tex) | [📊 EDA](B1_Fake_Job_Postings/figures/b1_eda.png) • [📈 Results](B1_Fake_Job_Postings/figures/b1_results.png) |
| **C2** | **BBC News Summarisation**<br>*(Abstractive Seq2Seq Fine-Tuning)* | [📓 `C2_notebook.ipynb`](C2_BBC_Summarisation/C2_notebook.ipynb) | [📄 `70177202_C2_Report.pdf`](C2_BBC_Summarisation/report/70177202_C2_Report.pdf) | [📝 `main.tex`](C2_BBC_Summarisation/report/source/main.tex) | [📊 EDA](C2_BBC_Summarisation/figures/c2_eda.png) • [📈 Results](C2_BBC_Summarisation/figures/c2_results.png) |

---

## 🏆 Experimental Highlights & Benchmark Summary

| Task | Dataset & Split | Winning Architecture | Primary Test Metrics | Key Engineering Insight |
| :---: | :--- | :--- | :--- | :--- |
| **A1** | **Breast Cancer Wisconsin**<br>`569` samples • `30` features<br>*(80% Train / 20% Test, 5-Fold CV)* | **Tuned Random Forest**<br>`100` trees, `max_depth=5`<br>Threshold `t = 0.26` | **F1:** `0.9630`<br>**ROC-AUC:** `0.9950`<br>**Recall:** `0.9524` | Lowering threshold from `0.50` to `0.26` raised malignant recall from `92.86%` to `95.24%` (`≥ 0.95` target). Naive correlation pruning hurt F1 (`0.9136`). |
| **B1** | **EMSCAD Job Postings**<br>`17,880` ads • `4.84%` fraud<br>*(70% Train / 15% Val / 15% Test)* | **Calibrated Linear SVM**<br>`C=0.5`, `20,077` features<br>Val Threshold `t = 0.40` | **Fraud F1:** `0.8618`<br>**PR-AUC:** `0.9404`<br>**ROC-AUC:** `0.9925` | Fusing TF-IDF `(