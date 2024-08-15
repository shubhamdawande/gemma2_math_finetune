# Gemma 2 Math Fine-tuning

This repository contains the fine-tuning process and results for a math-focused version of the Gemma 2 model.

## Dataset

We used the MathInstruct dataset for fine-tuning:

- **Dataset Name**: MathInstruct
- **Source**: [TIGER-Lab/MathInstruct on Hugging Face](https://huggingface.co/datasets/TIGER-Lab/MathInstruct)
- **Description**: MathInstruct is compiled from 13 math rationale datasets. It uniquely focuses on the hybrid use of chain-of-thought (CoT) and program-of-thought (PoT) rationales, and ensures extensive coverage of diverse mathematical fields.

## Base Model

Our fine-tuning process started with the following base model:

- **Model**: Gemma 2b Instruct
- **Version**: Unsloth's 4-bit quantized version
- **Source**: [unsloth/gemma-2b-it-bnb-4bit on Hugging Face](https://huggingface.co/unsloth/gemma-2b-it-bnb-4bit)

## Training Results

### Loss Curve

<img src="results/training_loss.svg" alt="Training Loss" width="450" height="300">

### Evaluation

We evaluated our fine-tuned model using Llama-3.1-70B as Judge. The results are visualized below:

<img src="results/comparison.png" alt="Training Loss" width="650" height="300">