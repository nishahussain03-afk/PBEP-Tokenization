# PBEP Tokenization and Autoregressive Language Model

## Abstract

This project implements a complete Natural Language Processing pipeline using Byte Pair Encoding (BPE) tokenization and an Autoregressive Causal Language Model (ARLM).

The tokenizer learns subword units from a training corpus and generates a vocabulary using iterative pair merging. The generated vocabulary is then used to tokenize text into numerical token IDs.

These token IDs are used to train a Transformer-based autoregressive language model capable of predicting the next token in a sequence.

---

# Objectives

The objectives of this project are:

- Implement Byte Pair Encoding from scratch.
- Learn merge rules automatically.
- Construct a subword vocabulary.
- Convert text into token IDs.
- Build a Transformer-based language model.
- Train the model using Cross Entropy Loss.
- Predict the next token.

---

# Methodology

## Step 1

Prepare the training corpus.

---

## Step 2

Initialize the vocabulary using characters.

---

## Step 3

Count adjacent token pairs.

---

## Step 4

Merge the most frequent token pair.

---

## Step 5

Repeat merging until the desired vocabulary size is reached.

---

## Step 6

Save

- vocabulary.txt
- merge_rules.txt

---

## Step 7

Convert text into token IDs.

---

## Step 8

Create training sequences.

Example

Input

```
machine learning enables computers
```

Target

```
to
```

---

## Step 9

Create embeddings.

---

## Step 10

Apply positional encoding.

---

## Step 11

Apply causal masking.

---

## Step 12

Train the Transformer encoder.

---

## Step 13

Predict the next token.

---

# Model Architecture

```
Input Text

↓

BPE Tokenizer

↓

Vocabulary

↓

Token IDs

↓

Embedding Layer

↓

Positional Encoding

↓

Transformer Encoder

↓

Linear Layer

↓

Softmax

↓

Next Token Prediction
```

---

# Technologies

- Python
- PyTorch
- NumPy
- Matplotlib
- Google Colab

---

# Results

The tokenizer successfully generated

- Vocabulary
- Merge Rules
- Token IDs

The language model successfully learned token relationships and predicted the next token from the given context.

Example

Input

```
machine learning
```

Prediction

```
enables
```

---

# Conclusion

The project demonstrates a complete implementation of Byte Pair Encoding and an Autoregressive Transformer Language Model.

The tokenizer effectively reduces unknown words by using subword units, while the Transformer captures contextual dependencies through causal self-attention for next-token prediction.

---

# Future Work

- Larger datasets
- Multi-GPU training
- Better text generation
- GPT-style decoder architecture
- Beam Search
- Top-k Sampling
