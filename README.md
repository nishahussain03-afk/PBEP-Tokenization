# PBEP Tokenization and Autoregressive Language Model

## Project Overview

This project implements **Byte Pair Encoding (BPE) Tokenization** and a **Transformer-based Autoregressive Causal Language Model (ARLM)** from scratch using Python and PyTorch.

The project demonstrates the complete NLP pipeline:

Raw Text
→ Byte Pair Encoding (BPE)
→ Vocabulary Creation
→ Merge Rules
→ Token IDs
→ Embedding Layer
→ Positional Encoding
→ Transformer Encoder
→ Causal Mask
→ Next Token Prediction

---

## Features

- Byte Pair Encoding (BPE) Tokenizer
- Vocabulary Construction
- Merge Rule Learning
- Tokenization using Learned Vocabulary
- Token ID Mapping
- Dataset Generation
- Positional Encoding
- Transformer-based Language Model
- Causal Self-Attention
- Cross Entropy Loss
- Adam Optimizer
- Text Generation

---

## Project Structure

```
PBEP-Tokenization/
│
├── BPE_Tokenizer.ipynb
├── ARLM_From_Scratch.ipynb
│
├── corpus.txt
├── vocabulary.txt
├── merge_rules.txt
│
├── arlm_model.pth
├── generated_text.txt
├── training_loss.png
│
├── README.md
├── report.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

## Technologies Used

- Python 3
- PyTorch
- NumPy
- Matplotlib
- Google Colab / Jupyter Notebook

---

## Installation

Clone the repository

```bash
git clone https://github.com/your-username/PBEP-Tokenization.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Running the Project

### Step 1

Open

```
BPE_Tokenizer.ipynb
```

Run all cells.

This generates:

- vocabulary.txt
- merge_rules.txt

---

### Step 2

Open

```
ARLM_From_Scratch.ipynb
```

Run all cells.

The notebook will

- Load the vocabulary
- Convert text into token IDs
- Create the training dataset
- Train the Transformer model
- Predict the next token

---

## Example

Input

```
machine learning
```

Output

```
enables
```

Example

```
artificial intelligence
```

Output

```
is
```

---

## Results

The project successfully implements:

- Byte Pair Encoding
- Vocabulary Learning
- Subword Tokenization
- Transformer-based Language Model
- Next Token Prediction

---

## Future Improvements

- Multi-head attention implementation from scratch
- Larger training corpus
- Beam Search
- Top-k Sampling
- Top-p Sampling
- Model evaluation using Perplexity

---

## Author

AFREEN NISHA 

University Name

Course: Natural Language Processing
