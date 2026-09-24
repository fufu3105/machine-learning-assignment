# Machine Learning Assignment - Group 8

[![Python](https://img.shields.io/badge/python-3.14.2-blue.svg)](https://www.python.org/) [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fufu3105/machine-learning-assignment/blob/main/assignment.ipynb)

---

<div align="center">
    <h2>Machine Learning Course Project — Group 8</h2>
    <h3>News Topic Classification</h3>
</div>

---

## Course Information

- **Course:** Machine Learning
- **Course Code:** CO3117
- **Semester:** 261, Academic Year 2026–2027
- **Instructor:** Dr. Trương Vĩnh Lân

---

## Team Members

| Name | Student ID | Email |
| --- | --- | --- |
| Nguyễn Tấn Khoa | 2352576 | [khoa.nguyen2352576@hcmut.edu.vn](mailto:khoa.nguyen2352576@hcmut.edu.vn) |
| Trương Hoàng Phú | 2352924 | [phu.truonghoang@hcmut.edu.vn](mailto:phu.truonghoang@hcmut.edu.vn) |
| Nguyễn Đức Thịnh | 2353140 | [thinh.nguyenthinh2503@hcmut.edu.vn](mailto:thinh.nguyenthinh2503@hcmut.edu.vn) |
| Lương Thế Kiệt | 2352649 | [kiet.luong1360@hcmut.edu.vn](mailto:kiet.luong1360@hcmut.edu.vn) |

---

## Project Overview

This project studies four-class news topic classification on the [AG News dataset](https://huggingface.co/datasets/fancyzhx/ag_news). It compares traditional text features and classifiers with pretrained embeddings, BiLSTM, and fine-tuned DistilBERT using common evaluation metrics and computational cost.

- **GitHub:** [fufu3105/machine-learning-assignment](https://github.com/fufu3105/machine-learning-assignment)
- **GitHub Pages:** [Github Pages](https://fufu3105.github.io/machine-learning-assignment/)
- **Dataset:** [AG News - Hugging Face](https://huggingface.co/datasets/fancyzhx/ag_news)
- **Report:** [Final report](https://github.com/fufu3105/machine-learning-assignment/blob/main/report/final_report.pdf)

---

## Project Target

- Inspect the AG News dataset and identify data-quality issues.
- Prepare reproducible training, validation, and test splits without data leakage.
- Compare Bag-of-Words, TF-IDF, and n-gram features.
- Evaluate Naive Bayes, Logistic Regression, Linear SVM, and Random Forest.
- Compare GloVe and frozen DistilBERT embeddings.
- Train a BiLSTM and fine-tune DistilBERT.
- Compare predictive performance, runtime, confusion patterns, and errors.

---

## Project Settings

### 1. Google Colab

Open notebook here: [Assignment](https://colab.research.google.com/github/fufu3105/machine-learning-assignment/blob/main/assignment.ipynb)

### 2. Local Run

```bash
# Clone repository
git clone https://github.com/fufu3105/machine-learning-assignment.git
cd machine-learning-assignment

# Optional: create a virtual environment
python -m venv venv
venv\Scripts\activate           # Windows  
# source venv/bin/activate          # Linux / macOS

# Upgrade pip
python -m pip install --upgrade pip

# Install dependencies
python -m pip install -r requirements.txt

# Start Jupyter Notebook
jupyter notebook assignment.ipynb
```

---

## Repository Structure

```text
machine-learning-assignment/
├── data/                   # Dataset cache
│   ├── raw/                
│   └── processed/          
├── features/               # Extracted features
│   ├── bow/                
│   ├── tfidf/              
│   ├── glove/              
│   └── distilbert/         
├── models/                 # Model checkpoints
├── results/                # Experiment outputs
│   ├── figures/            
│   ├── metrics/           
│   └── tables/             
├── report/                 # Final report
├── docs/                   # GitHub Pages site
├── assignment.ipynb        
├── requirements.txt        
├── README.md              
└── .gitignore             
```

---

## References

- [AG News dataset on Hugging Face](https://huggingface.co/datasets/fancyzhx/ag_news)
- [Scikit-learn text feature extraction](https://scikit-learn.org/stable/modules/feature_extraction.html#text-feature-extraction)
- [Gensim Downloader API](https://radimrehurek.com/gensim/downloader.html)
- [GloVe: Global Vectors for Word Representation](https://nlp.stanford.edu/projects/glove/)
- [DistilBERT documentation](https://huggingface.co/docs/transformers/model_doc/distilbert)
- [DistilBERT paper](https://arxiv.org/abs/1910.01108)
- [PyTorch LSTM documentation](https://docs.pytorch.org/docs/stable/generated/torch.nn.LSTM.html)
