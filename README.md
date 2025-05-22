# Natural Language Processing with NLTK

This repository contains a Jupyter notebook demonstrating basic Natural Language Processing (NLP) techniques using the Natural Language Toolkit (NLTK) in Python.

## Overview

The notebook (`NLP_test.ipynb`) explores fundamental NLP concepts and techniques including:

- **Tokenization**: Breaking text into sentences and words
- **Stop Word Removal**: Filtering out common words that add little meaning
- **Stemming**: Reducing words to their root form
- **Parts of Speech (POS) Tagging**: Identifying grammatical parts of speech

## Features

- Sentence tokenization with `sent_tokenize`
- Word tokenization with `word_tokenize`
- Filtering stop words using NLTK's English stopwords corpus
- Word stemming with Porter Stemmer
- POS tagging to identify grammatical elements

## Requirements

- Python 3.x
- NLTK library
- Jupyter Notebook

## Installation

```bash
# Install required packages
pip install nltk jupyter

# Download necessary NLTK data
python -c "import nltk; nltk.download('punkt'); nltk.download('stopwords')"
```

## Usage

1. Clone this repository
2. Open the Jupyter notebook:
   ```bash
   jupyter notebook NLP_test.ipynb
   ```
3. Run the cells to see the NLP techniques in action

## Example Code

```python
# Tokenizing text into sentences
from nltk.tokenize import sent_tokenize
example_text = "This is a sample sentence. This is another sentence."
sentences = sent_tokenize(example_text)

# Tokenizing text into words
from nltk.tokenize import word_tokenize
words = word_tokenize(example_text)

# Removing stop words
from nltk.corpus import stopwords
stop_words = set(stopwords.words("english"))
filtered_words = [word for word in words if word.casefold() not in stop_words]
```

## References

- Based on tutorials from [Real Python](https://realpython.com/nltk-nlp-python/)
- [NLTK Documentation](https://www.nltk.org/)

## License

MIT

## Author

Alan John A