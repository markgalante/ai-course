# NLP Course Notebooks

This repository contains Jupyter notebooks and practical exercises for an NLP (Natural Language Processing) course. It covers common text-processing techniques and modern NLP tooling using Python.

The project is designed to be **easy to set up**, **reproducible**, and **safe to version-control** (the virtual environment is intentionally excluded from git).

---

## 📁 Project Structure

```
.
├── practicals/                 # Practical exercises / assignments
├── *.ipynb                     # Course notebooks
├── requirements.txt            # Python dependencies
├── README.md                   # Project documentation
└── .gitignore                  # Git ignore rules (venv, caches, etc.)
```

> Note: The local virtual environment directory (`nlp-course-env/`) and Jupyter checkpoints are **not committed**.

---

## 🐍 Python Version

Recommended:

* **Python 3.11+**

You can check your version with:

```bash
python --version
```

---

## ⚙️ Environment Setup

### 1. Create a virtual environment

From the project root:

```bash
python -m venv nlp-course-env
```

Activate it:

* **macOS / Linux**

  ```bash
  source nlp-course-env/bin/activate
  ```

* **Windows**

  ```powershell
  nlp-course-env\Scripts\activate
  ```

---

### 2. Install dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

This installs all required NLP, ML, and Jupyter packages.

---

## 📦 Key Libraries Used

* **NumPy / Pandas** – numerical & tabular data
* **NLTK / spaCy / TextBlob** – classical NLP
* **scikit-learn** – ML utilities
* **Transformers** – modern NLP models (Hugging Face)
* **Gensim** – topic modeling & embeddings
* **PyTorch** – deep learning backend
* **Matplotlib / Seaborn** – visualization
* **JupyterLab / Notebook** – interactive development

---

## 📘 spaCy Language Models

spaCy language models are **not installed automatically** via `requirements.txt`.

If a notebook requires one, install it manually, for example:

```bash
python -m spacy download en_core_web_sm
```

---

## 📚 NLTK Data

Some notebooks may download NLTK datasets at runtime, e.g.:

```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
```

This is expected behavior.

---

## ▶️ Running the Notebooks

Start Jupyter Lab:

```bash
jupyter lab
```

or the classic notebook interface:

```bash
jupyter notebook
```

Then open the desired `.ipynb` file in your browser.

---

## 🧹 Git Hygiene

Ignored files/directories include:

* Virtual environment (`nlp-course-env/`)
* Jupyter checkpoints (`.ipynb_checkpoints/`)
* Python cache files (`__pycache__/`)

Dependencies are tracked via `requirements.txt`.

---

## 📝 Notes

* This repository is intended for **learning and experimentation**.
* Notebooks may be exploratory and are not optimized for production use.

---

## ✅ Quick Start (TL;DR)

```bash
python -m venv nlp-course-env
source nlp-course-env/bin/activate
pip install -r requirements.txt
jupyter lab
```