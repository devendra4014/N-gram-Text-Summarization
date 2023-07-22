# Text Summarization using N-gram Algorithm

![Text Summarization](https://example.com/text-summarization.png)

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Installation](#installation)
- [Algorithm](#algorithm)
- [Example](#example)

## Introduction

This project implements a text summarization system using the N-gram algorithm. Text summarization is the process of generating a concise and coherent summary of a longer document or text. The N-gram algorithm is a statistical language model that identifies recurring sequences of N words in a given text and uses these sequences to generate summaries.

The goal of this project is to demonstrate how N-grams can be leveraged for text summarization and provide a simple and effective summarization tool for anyone working with textual data.

## Requirements

To run this project, you will need the following:

- Python 3.x
- NumPy (for efficient array manipulation)
- PyPDF2

## Installation

1. Install the required dependencies:

   ```
   pip install numpy
   ```



## Algorithm

The N-gram algorithm works by tokenizing the input text into individual words and then extracting sequences of N words (N-grams). These N-grams are ranked based on their frequency in the text, and the most frequent ones are used to construct the summary. Shorter, more frequent N-grams are given higher importance.

The Relative Probability Formula for N-gram Algorithm:

Given a sequence of words or tokens, the relative probability of an n-gram (a sequence of n consecutive words or tokens) can be calculated as follows:

P(word_n | word_1, word_2, ..., word_(n-1)) = Count(word_1, word_2, ..., word_n) / Count(word_1, word_2, ..., word_(n-1))

Where:
- P(word_n | word_1, word_2, ..., word_(n-1)) is the relative probability of word_n given the context of the preceding n-1 words.
- Count(word_1, word_2, ..., word_n) is the number of occurrences of the n-gram (word_1, word_2, ..., word_n) in the training data.
- Count(word_1, word_2, ..., word_(n-1)) is the number of occurrences of the (n-1)-gram (word_1, word_2, ..., word_(n-1)) in the training data.

The n-gram algorithm is commonly used in natural language processing and statistical language modeling tasks to estimate the likelihood of word sequences based on their occurrences in the training data.

## Example

Suppose we have the following input text:

```
"The quick brown fox jumps over the lazy dog. The dog barks at the moon. The fox and the dog become friends under the moonlight."
```

Using the N-gram algorithm with N=2, the summary might be:

```
"The quick brown fox jumps over the lazy dog. The dog barks at the moon."
```
NSE).
