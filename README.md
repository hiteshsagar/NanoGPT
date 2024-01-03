# Char-RNN Language Model

This repository contains a character-level language model implemented in PyTorch. The model is trained on the Tiny Shakespeare dataset to generate text.

## Overview

- The language model is based on a Transformer architecture with self-attention mechanisms.
- It uses a bigram approach to predict the next token in a sequence.
- Training and evaluation are performed on the Tiny Shakespeare dataset.
- The model is implemented in PyTorch and utilizes GPU acceleration if available.

## Hyperparameters

- Batch Size: 16
- Block Size: 32
- Max Iterations: 5000
- Evaluation Interval: 100
- Learning Rate: 1e-3
- Device: CUDA (if available), otherwise CPU
- Evaluation Iterations: 200
- Embedding Dimension: 64
- Number of Heads: 4
- Number of Layers: 4
- Dropout: 0.0

## How to Use

1. Install the required dependencies using `pip install torch`.
2. Download the Tiny Shakespeare dataset (`input.txt`) from [here](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt).
3. Run the provided Python script to train the language model.

```bash
python language_model.py
