# Simple LLM Implementation

This project provides an introductory walkthrough of basic Natural Language Processing (NLP) concepts using the **spaCy** library, as well as comparisons with other popular NLP libraries. It is ideal for those who are beginning their journey with Large Language Models (LLMs) and want to understand tokenization, embeddings, and vector space representations.

## 📘 Overview

In this notebook, you will learn about:

- Key NLP concepts: **Token**, **Vocab**, **Sequence**
- Introduction to **spaCy** and its major features
- Installing and using `en_core_web_md`, a medium-sized English language model
- Performing tasks such as:
  - Tokenization
  - Accessing word vectors
  - Understanding similarity between words
- Comparison with other libraries such as Hugging Face Transformers, NLTK, Stanza, Flair, Gensim, AllenNLP, and TextBlob

## 🛠️ Technologies Used

- **Python 3**
- **spaCy**: Industrial-strength NLP library
- Jupyter Notebook for code and documentation

## 📦 Installation

To run this notebook:

1. Install required libraries:
   ```bash
   pip install spacy
   ```

2. Download the spaCy English model:
   ```bash
   python -m spacy download en_core_web_md
   ```

3. Open the notebook in Jupyter and follow along with the code and explanations.

## ✨ Features Demonstrated

- Tokenization and vector inspection using spaCy
- Embedding text into a vector space
- Semantic similarity demonstration
- Library comparison to help decide the best tool for your NLP use case

## 🔍 Example

```python
import spacy
nlp = spacy.load("en_core_web_md")
doc = nlp("Apple is looking at buying U.K. startup for $1 billion")

for token in doc:
    print(token.text, token.has_vector, token.vector_norm)
```

## 📚 Further Reading

- [spaCy Documentation](https://spacy.io/usage)
- [Hugging Face Transformers](https://huggingface.co/transformers/)
- [NLTK](https://www.nltk.org/)
- [Stanford NLP / Stanza](https://stanfordnlp.github.io/stanza/)
- [Flair](https://github.com/flairNLP/flair)

## 🧠 Author Notes

This notebook is a foundation for deeper LLM explorations. It's a good starting point before transitioning to more complex models and workflows using Hugging Face or TensorFlow.
