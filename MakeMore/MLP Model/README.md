# Makemore MLP (Lecture 3)

## Overview

This notebook contains an implementation of a character-level language
model using a Multi-Layer Perceptron (MLP), based on Andrej Karpathy's
Makemore Lecture 3.

The goal is to predict the next character in a name given a fixed-length
context window.

## Key Concepts Covered

-   Character-level dataset preparation\
-   Building input-output pairs using context window (block size)\
-   Embedding layer for character representation\
-   Flattening embeddings before feeding into the MLP\
-   Hidden layer with tanh activation\
-   Output layer producing logits over vocabulary\
-   Training using cross entropy loss\
-   Manual gradient descent parameter updates\
-   Importance of initialization for stable training

## Model Architecture

Input context -\> Embedding lookup -\> Flatten -\> Linear + tanh -\>
Linear -\> Vocabulary logits -\> Cross entropy loss

## Files

MakeMore_MLP.ipynb : Main notebook implementing the MLP model

## How to Run

Open the notebook in Jupyter or Google Colab and run cells in order.

## Output

The notebook trains an MLP-based character model and generates new
name-like sequences by sampling from the learned probability
distribution.

## Reference

Based on Andrej Karpathy's Makemore series Lecture 3.
