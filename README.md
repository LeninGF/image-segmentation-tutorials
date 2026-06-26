# Image Segmentation Tutorials

Experiments with transformer-based image segmentation models for my PhD thesis.

## Contents

- **`image_segmentation_tutorial.ipynb`** — Introduction to semantic and interactive segmentation using [SegFormer](https://arxiv.org/abs/2105.01601) (NVIDIA) and [Segment Anything Model (SAM)](https://arxiv.org/abs/2304.02643) (Meta). Covers loading pretrained models from Hugging Face, running inference, and comparing the two approaches.

- **`Fine-Tuning-SemanticSegmentation.ipynb`** — Fine-tuning a SegFormer model (`nvidia/mit-b0`) on a custom semantic segmentation dataset from the Hugging Face Hub. Uses the `segments/sidewalk-semantic` dataset and trains with the Hugging Face `Trainer` API.

## Environment Setup

1. Install dependencies (PyTorch, Transformers, datasets, evaluate, etc.)
2. Create a `.env` file with your Hugging Face token: `HF_TOKEN=hf_your_read_token_here`
3. Run the notebooks in order.

## Notes

- These notebooks were developed and tested on an internal lab GPU server.
- The `.env` file is gitignored — your tokens stay local.
- Model checkpoints and output directories are not tracked in this repository.
