# README

## Project: MakeMore Manual Backpropagation

This project follows Andrej Karpathy’s *MakeMore* lecture series and implements manual backpropagation for a character-level language model.

The goal is to understand how neural networks compute gradients internally instead of relying only on PyTorch autograd.

---

## Contents

- Character-level dataset preparation  
- Bigram and MLP-based language model  
- Forward pass implementation  
- Manual backpropagation step-by-step  
- Gradient verification with PyTorch autograd  
- Training loop and loss optimization  

---

## Key Concepts Covered

- Logits, softmax, and cross entropy loss  
- Embedding lookup (`emb = C[X]`)  
- Tensor shapes in batch and block processing  
- Gradient flow through lookup tables  
- Manual computation of derivatives  
- Comparing manual gradients with autograd  

---

## Files

- `MakeMore_manual_Backprop.ipynb`  
  Main notebook containing forward and backward implementations.

---

## How to Run

1. Open the notebook in Jupyter or Google Colab  
2. Run cells sequentially  
3. Observe loss decrease and gradient checks  

---

## Objective

To build strong intuition for:

- How backpropagation works internally  
- How embeddings receive gradients  
- How language models learn next-token prediction  
