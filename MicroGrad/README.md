# Micrograd and PyTorch Basics (Stage 1 LLM Foundations)

This folder contains my early Stage 1 learning work toward understanding Large Language Models from scratch.

Instead of jumping directly into high-level libraries, I focused on building the foundations first:

- Understanding how backpropagation works internally  
- Learning how neural networks compute gradients  
- Connecting PyTorch abstractions to the underlying mathematics  

These notebooks are based on Andrej Karpathy’s Neural Networks: Zero to Hero approach and are part of my Stage 1 roadmap toward Transformers and GPT-style models.

---

## Notebooks Included

### 1. Micrograd_from_Scratch.ipynb

In this notebook, I implemented a minimal autograd engine similar to PyTorch’s internal core.

Key concepts learned:

- Building a Value class to store:
  - data
  - gradients
  - computation graph dependencies
- Implementing forward operations:
  - addition, multiplication
  - tanh, exp
- Writing custom backward functions for each operation
- Understanding the chain rule through manual backpropagation
- Visualizing computation graphs using Graphviz (draw_dot)

This notebook helped me understand that gradients are not magic, but repeated applications of the chain rule.

---

### 2. Pytorch_basics_micrograd_ops_here.ipynb

This notebook connects micrograd fundamentals to real PyTorch workflows.

Topics covered:

- Tensor basics and dtype issues (float32 vs float64)
- Training loop structure:
  - forward pass
  - loss computation
  - backward pass
  - optimizer step
- Binary classification loss pitfalls:
  - BCELoss vs CrossEntropyLoss
  - label dtype requirements (float vs long)
- Debugging common errors in neural network training
- Understanding why preprocessing and tensor types matter

This notebook helped bridge the gap between building neural networks from scratch and training models using PyTorch.

---

## Why This Matters for LLMs

Stage 1 of my LLM roadmap focuses on building strong fundamentals before moving to Transformers.

Micrograd teaches:

- how gradients flow
- how optimization works internally

PyTorch basics teach:

- how these ideas scale to real deep learning models

These concepts are essential before studying:

- Attention mechanisms
- Transformers
- GPT training from scratch

Next steps include implementing a Bigram Language Model, moving toward Transformer blocks, and building a character-level GPT.

---

## Tools Used

- Python
- PyTorch
- Graphviz
- Jupyter Notebook

---

## Next Steps

- Implement Bigram Language Model from scratch
- Study attention and Transformer architecture
- Build a character-level GPT model in PyTorch

---

## Reference

This work is part of Stage 1 resources:

- CampusX PyTorch Foundations  
- Andrej Karpathy: Neural Networks Zero to Hero  
- StatQuest Transformer Intuition  

