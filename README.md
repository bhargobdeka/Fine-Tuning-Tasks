# Fine-Tuning-Tasks

This repository contains coding tutorials on fine-tuning transformer models, either full or parameter efficient.

## Project 1: Fine-tuning a Vision Transformer for Houseplant Image Classification

![My HF spaces app for houseplant health check](full-finetuning-ViT.gif)

### Model

This model is a fine-tuned version of google/vit-base-patch16-224-in21k on the [houseplant image dataset](https://huggingface.co/datasets/bhargob11/houseplants). It achieves the following results on the evaluation set:

- Loss: 0.4007
- Accuracy: 0.8673

You can download the model from my [profile](https://huggingface.co/bhargob11).

### Notebook

The repo contains two notebook files where I performed experiments with both full finetuning a vision transformer for the image classification task as well as parameter efficient finetuning (PEFT) using QLORA. The PEFT model leads to poorer accuracy compared to the full one, suggesting that full fine tuning is necessary in this case. Here are the two files:

- notebooks/Full_fine_tuning_image_classification_houseplant.ipynb
- notebooks/PEFT_fine_tuning_image_classification_houseplant.ipynb

### Framework versions

- Transformers 4.42.4
- Pytorch 2.3.1+cu121
- Datasets 2.21.0
- Tokenizers 0.19.1
