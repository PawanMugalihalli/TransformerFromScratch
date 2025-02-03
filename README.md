# Transformer Network Implementation from Scratch (PyTorch)

This repository contains an implementation of the Transformer architecture from scratch, inspired by the paper ["Attention Is All You Need"](https://arxiv.org/abs/1706.03762), using PyTorch. The model is designed to perform sequence-to-sequence tasks such as translation or text generation.

## Key Features

- **Self-attention mechanism**: Efficiently computes relationships between tokens in a sequence.
- **Positional encoding**: Adds position information to the input embeddings to account for token order.
- **Encoder-decoder architecture**: Uses multiple layers of encoder and decoder blocks for sequence-to-sequence tasks.
- **Multi-head attention**: Allows the model to attend to different parts of the sequence simultaneously, improving learning of complex patterns.
- **Masking**: Implements masking to prevent attention to certain tokens, useful for tasks like sequence generation.

## Model Details

- **Number of layers**: 6
- **Number of attention heads**: 8
- **Embedding size**: 512
- **Dropout rate**: 0
- **Forward expansion**: 4 (for the feed-forward layers)

## Requirements

Ensure you have the following dependencies installed:

```sh
pip install torch numpy matplotlib
```

- Python 3.7+
- PyTorch 1.8+
- NumPy
- Matplotlib (for visualization, if needed)

## Usage

To train the Transformer model, run the following command:

```sh
python train.py
```

For inference:

```sh
python predict.py --input "your input sequence"
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

