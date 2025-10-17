# DistilBERT Sentiment Classification: Full Fine-Tuning vs LoRA

This repository contains code and results for Chinese sentiment classification experiments using DistilBERT on the ChnSentiCorp dataset, comparing traditional full fine-tuning with parameter-efficient LoRA methods.

## Overview

- **Task**: Binary sentiment classification on Chinese texts
- **Base Model**: DistilBERT-base-chinese via BertForSequenceClassification
- **Datasets**: [Lansinuote/ChnSentiCorp](https://huggingface.co/datasets/lansinuote/ChnSentiCorp)
- **Methods**:
  - Full Fine-Tuning (all parameters)
  - LoRA (Low-Rank Adaptation of attention layers)

## Results

| Method                  | Trainable Params | Test Accuracy | Test F1 Score |
|-------------------------|------------------|---------------|---------------|
| Full Fine-Tuning        | 109,780,228      | 0.7142        | 0.7142        |
| LoRA (rank=8, α=16)     | 296,450          | 0.5208        | 0.3833        |

## File Structure

- `Assignment3-3.ipynb`: Main Jupyter notebook with experiment code and results

## Usage

Direct run the code chunks in the notebook. And you need to change the file path to your own.

## tips

In the Github you may see this:
<img width="681" height="248" alt="image" src="https://github.com/user-attachments/assets/8fbd5ce6-7b19-4458-940a-66b4a331173b" />

Just download it and you can get the good file.

