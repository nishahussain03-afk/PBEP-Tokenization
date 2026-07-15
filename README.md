# Byte Pair Encoding (BPE) Tokenizer from Scratch

## Project Overview

This project implements a **Byte Pair Encoding (BPE) Tokenizer** completely from scratch using Python in JupyterLab. The tokenizer learns subword vocabulary by repeatedly merging the most frequent adjacent symbol pairs found in a text corpus.

This implementation does not use any external tokenizer libraries such as Hugging Face Tokenizers or SentencePiece. Every step of the BPE algorithm is implemented manually.

---

## Objective

The objective of this project is to understand how Byte Pair Encoding works internally by implementing every stage of the algorithm, including:

- Reading a text corpus
- Preprocessing text
- Character-level tokenization
- Word frequency calculation
- Pair frequency calculation
- Learning merge rules
- Building vocabulary
- Encoding unseen words
- Decoding encoded tokens

---

## Features

- Custom text corpus
- Automatic vocabulary generation
- Pair frequency counting
- Iterative merge operations
- Learned merge rules
- Character-level tokenizer
- BPE encoder
- BPE decoder
- Final vocabulary generation
- Sample testing on unseen words

---

## Project Structure

```
PBEP-Tokenization/
│
├── BPE_Tokenizer.ipynb
├── corpus.txt
├── merge_rules.txt
├── vocabulary.txt
├── sample_output.txt
├── README.md
├── report.md
├── requirements.txt
└── LICENSE
```

---

## Algorithm

The implementation follows these steps:

1. Create Corpus
2. Read Corpus
3. Preprocess Text
4. Split Words into Characters
5. Count Word Frequencies
6. Find Adjacent Symbol Pairs
7. Count Pair Frequencies
8. Select Most Frequent Pair
9. Merge Pair
10. Update Vocabulary
11. Repeat Merge Process
12. Save Merge Rules
13. Build Final Vocabulary
14. Encode New Words
15. Decode Tokens
16. Test the Tokenizer
17. Display Results

---

## Technologies Used

- Python 3.x
- JupyterLab
- collections
- re

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/PBEP-Tokenization.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch JupyterLab

```bash
jupyter lab
```

Open

```
BPE_Tokenizer.ipynb
```

Run all cells.

---

## Sample Output

```
Merge 1 : ('i', 'n')

Merge 2 : ('e', 'r')

Merge 3 : ('t', 'i')

...

Vocabulary Size : 85

Encoding

tokenization

↓

['to', 'ken', 'ization', '</w>']

Decoded

tokenization
```

---

## Learning Outcomes

This project demonstrates:

- Tokenization from scratch
- Data preprocessing
- Frequency analysis
- Greedy pair merging
- Vocabulary learning
- NLP preprocessing techniques

---

## Future Improvements

- Token IDs
- Unknown token support
- Save and load trained tokenizer
- Larger datasets
- Performance optimization
- Sentence-level encoding

---

## Author

Afreen Nisha 
