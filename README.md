\# AI101-ML-Assignment-70177202



\*\*Student Name:\*\* Aliaan Shams  

\*\*Roll Number:\*\* 70177202  

\*\*Section:\*\* C  

\*\*Course:\*\* AI-101 — Machine Learning (Department of Intelligent Systems, The University of Lahore)  

\*\*Instructor:\*\* Dr. Muhammad Awais, AI Architect  

\*\*Selected Tasks:\*\* A1, B1, C2  



\---



\## Repository Overview



This repository contains end-to-end, leakage-free machine learning and NLP implementations, evaluation figures, and 2-page IEEE conference reports for three tasks:



| Task | Title | Dataset | Best Model \& Configuration | Key Test Results | Notebook | IEEE Report |

| :--- | :--- | :--- | :--- | :--- | :--- | :--- |

| \*\*A1\*\* | Breast Cancer Diagnosis | Breast Cancer Wisconsin (Diagnostic) (`sklearn` / UCI ID 17) | Tuned Random Forest (`n\_estimators=100`, `max\_depth=5`, threshold `0.26`) | F1: \*\*0.9630\*\* \\| ROC-AUC: \*\*0.9950\*\* \\| Recall: \*\*0.9524\*\* | \[A1\_notebook.ipynb](A1\_Breast\_Cancer/A1\_notebook.ipynb) | \[70177202\_A1\_Report.pdf](A1\_Breast\_Cancer/report/70177202\_A1\_Report.pdf) |

| \*\*B1\*\* | Fraudulent Job Posting Detection | Employment Scam Aegean Dataset (EMSCAD, Kaggle) | Calibrated Linear SVM (`C=0.5`, TF-IDF + Metadata, threshold `0.40`) | Fraud F1: \*\*0.8618\*\* \\| PR-AUC: \*\*0.9404\*\* \\| ROC-AUC: \*\*0.9925\*\* | \[B1\_notebook.ipynb](B1\_Fake\_Job\_Postings/B1\_notebook.ipynb) | \[70177202\_B1\_Report.pdf](B1\_Fake\_Job\_Postings/report/70177202\_B1\_Report.pdf) |

| \*\*C2\*\* | Abstractive News Summarisation | BBC News Summary (`gopalkalpande/bbc-news-summary`, Hugging Face) | Fine-Tuned `t5-small` (3 epochs, Beam=4, 3-gram blocking) | ROUGE-1: \*\*53.56\*\* \\| ROUGE-2: \*\*44.77\*\* \\| ROUGE-L: \*\*40.31\*\* | \[C2\_notebook.ipynb](C2\_BBC\_Summarisation/C2\_notebook.ipynb) | \[70177202\_C2\_Report.pdf](C2\_BBC\_Summarisation/report/70177202\_C2\_Report.pdf) |



\---



\## Repository Structure



```text

AI101-ML-Assignment-70177202/

├── A1\_Breast\_Cancer/

│   ├── A1\_notebook.ipynb

│   ├── data/

│   ├── figures/

│   └── report/

│       ├── 70177202\_A1\_Report.pdf

│       └── source/main.tex

├── B1\_Fake\_Job\_Postings/

│   ├── B1\_notebook.ipynb

│   ├── data/

│   ├── figures/

│   └── report/

│       ├── 70177202\_B1\_Report.pdf

│       └── source/main.tex

├── C2\_BBC\_Summarisation/

│   ├── C2\_notebook.ipynb

│   ├── figures/

│   └── report/

│       ├── 70177202\_C2\_Report.pdf

│       └── source/main.tex

├── AI\_DISCLOSURE.md

├── README.md

└── requirements.txt

