# Byte Pair Encoding (BPE) Tokenizer from Scratch

## Abstract

Byte Pair Encoding (BPE) is one of the most widely used subword tokenization techniques in Natural Language Processing (NLP). It reduces the vocabulary size while preserving meaningful subword units. This project implements the complete BPE algorithm from scratch using Python without relying on any external tokenizer libraries.

---

# Objective

The objective of this project is to understand and implement every stage of the Byte Pair Encoding algorithm manually, including vocabulary construction, pair merging, encoding, and decoding.

---

# Implementation Steps

## Step 1: Create a Text Corpus

A custom corpus consisting of technology-related words was created.

Example:

```
artificial
machine
learning
transformer
tokenization
attention
language
```

---

## Step 2: Read the Corpus

The corpus was stored in a text file and loaded into Python.

---

## Step 3: Preprocess Text

The following preprocessing operations were performed:

- Convert to lowercase
- Remove unnecessary whitespace
- Clean unwanted symbols

---

## Step 4: Character-Level Tokenization

Each word was split into characters.

Example

```
machine

↓

m a c h i n e </w>
```

The end-of-word marker (`</w>`) preserves word boundaries.

---

## Step 5: Count Word Frequencies

A dictionary was created to count the occurrence of each unique word representation.

---

## Step 6: Find Adjacent Symbol Pairs

Adjacent symbols were extracted.

Example

```
m a c h i n e </w>

Pairs

(m,a)
(a,c)
(c,h)
(h,i)
(i,n)
(n,e)
(e,</w>)
```

---

## Step 7: Count Pair Frequencies

The frequency of each adjacent pair was calculated across the entire vocabulary.

---

## Step 8: Select the Most Frequent Pair

The pair with the highest frequency was selected for merging.

---

## Step 9: Merge the Pair

The selected pair was merged into a new token.

Example

```
i n

↓

in
```

---

## Step 10: Update Vocabulary

Every occurrence of the merged pair was replaced in the vocabulary.

---

## Step 11: Repeat Merge Process

The merge operation was repeated for a fixed number of iterations until the desired vocabulary size was reached.

---

## Step 12: Store Merge Rules

Every merge operation was stored in order.

These merge rules were later used during encoding.

---

## Step 13: Build Final Vocabulary

The final vocabulary consists of:

- Individual characters
- Merged subwords
- End-of-word symbol

---

## Step 14: Implement Encoder

The encoder applies the learned merge rules sequentially to tokenize new words into subword tokens.

---

## Step 15: Implement Decoder

The decoder reconstructs the original word by concatenating the generated tokens and removing the end-of-word marker.

---

## Step 16: Test the Tokenizer

The tokenizer was evaluated using unseen words such as:

- transformer
- chatbot
- prediction
- language
- tokenization

Both encoding and decoding produced the expected results.

---

## Step 17: Display Results

The implementation displays:

- Learned vocabulary
- Merge rules
- Encoded words
- Decoded words
- Vocabulary size

---

# Results

The tokenizer successfully learned frequent subword units from the corpus. The learned merge rules enabled efficient tokenization of unseen words while preserving meaningful subword structures.

---

# Conclusion

This project demonstrates a complete implementation of the Byte Pair Encoding (BPE) algorithm from scratch. It provides a clear understanding of vocabulary learning, subword tokenization, and encoding/decoding mechanisms commonly used in modern NLP models such as GPT, BERT, and RoBERTa.

---

# References

1. Sennrich, Haddow & Birch (2016). Neural Machine Translation of Rare Words with Subword Units.

2. Hugging Face Tokenizers Documentation

3. OpenAI Tokenization Concepts

4. Byte Pair Encoding Algorithm
