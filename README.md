# One-Hot Encoding of Words and Characters

This Python notebook demonstrates the concept of **One-Hot Encoding** applied to both words and individual characters using the `numpy` library. One-hot encoding is a common technique used in Natural Language Processing (NLP) and machine learning to convert categorical data (like words or characters) into a numerical format that models can understand.

## Project Overview

The notebook covers two main examples:

1.  **One-Hot Encoding for Words:**
    * Takes a simple sentence ("the cat sat on the mat") as input.
    * Creates a vocabulary of unique words from the sentence.
    * Assigns a unique index to each word in the vocabulary.
    * Generates a matrix where each row represents a word from the original sentence. In each row, the element corresponding to the word's index is set to `1`, and all other elements are set to `0`.

2.  **One-Hot Encoding for Characters:**
    * Takes a simple word ("hello") as input.
    * Creates a vocabulary of unique characters from the word.
    * Assigns a unique index to each character.
    * Generates a matrix where each row represents a character from the original word, encoded in a one-hot vector format based on its index.

## What is One-Hot Encoding?

One-hot encoding represents categorical variables as binary vectors. The key idea is:
* Create a vector with the same length as the number of unique categories (the vocabulary size).
* For a specific item (word or character), place a `1` at the index corresponding to that item in the vocabulary.
* Place `0`s in all other positions.

**Example (Words):**
If the vocabulary is `['cat', 'mat', 'on', 'sat', 'the']`, the word "cat" (index 0) would be represented as `[1, 0, 0, 0, 0]`.

**Example (Characters):**
If the character vocabulary for "hello" is `['e', 'h', 'l', 'o']`, the character 'h' (index 1) would be `[0, 1, 0, 0]`.

---

## Requirements

* `numpy`

You can install it using pip:
```bash
pip install numpy
