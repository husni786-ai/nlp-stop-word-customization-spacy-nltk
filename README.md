

**`nlp-stop-word-customization-spacy-nltk`**

---

# 🗑️ Stop Word Management in NLP (spaCy & NLTK)

This project provides a Jupyter Notebook demonstrating essential Natural Language Processing (NLP) text cleaning techniques, focusing specifically on **stop word removal** and **tokenization** using the popular `spaCy` and `nltk` libraries. Crucially, it illustrates how to inspect and customize the stop word lists for specific analytical needs.

## 🎯 Project Goals

The primary objective of this notebook is to showcase the pipeline for text preprocessing, with an emphasis on stop word management:

1.  **Initialize NLP Tools:** Load the `spaCy` model (`en_core_web_sm`) and download `nltk` resources.
2.  **Inspect Default Lists:** View and count the default stop words provided by `spaCy`.
3.  **Customize Stop Words:** Demonstrate how to dynamically add custom words (e.g., `'husnain'`) to the `spaCy` stop word vocabulary and set their stop flag.
4.  **Tokenization and Cleaning:** Process a sample sentence through tokenization, lowercasing, punctuation removal (using `re` and `string`), and final stop word filtering (using the `nltk` corpus).

## ⚙️ Technology Stack and Dependencies

The project relies on standard Python libraries for NLP and data handling.

| Library | Role |
| :--- | :--- |
| **`spaCy`** | Used for efficient model loading, stop word list access, and vocabulary customization. |
| **`nltk`** | Used for downloading the standard English stop word corpus and performing word tokenization. |
| **`string` / `re`** | Standard Python modules used for efficient punctuation detection and removal. |

### Installation

To run this notebook, you must install `spaCy` and download its language model.

```bash
# Install spaCy and its small English model
pip install spacy
python -m spacy download en_core_web_sm

# The notebook will automatically handle NLTK downloads (stopwords, punkt)
pip install nltk
