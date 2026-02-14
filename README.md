# Figurative-Language-Understanding

The official repository for the project of Deep Natural Language Processing 2025/2026, group 23: "Transformers".

## About our work

This repository implements and evaluates advanced Sentiment Analysis and Sarcasm Detection models across three English varieties (British, Australian, and Indian) using the BESSTIE benchmark. We compare the performance of an encoder model (BERT-large-uncased) against a generative Large Language Model (Mistral-7B-Instruct-v0.3). The project explores several architectural extensions to the base models, including Multitask Learning with Dynamic Loss Weighting, Supervised Contrastive Learning and Data Augmentation (Back-Translation & Synonym Replacement) for BERT, alongside QLoRA Fine-Tuning, Few-Shot Prompting and Probing strategy for Mistral. All models are optimized with 4-bit quantization for resource-constrained environments.


## Project structure

```text
├── Dataset/ 
│   ├── train.csv # training dataset from BESSTIE paper
│   ├── valid.csv # validation dataset from BESSTIE paper
│   ├── Augmented/
|   |   ├── train_augmented_BT-LLM.csv # training dataset augmented with back-translation strategy
|   |   ├── train_augmented_Swap.csv   # training dataset augmented with synonym replacement strategy
├── BERT/    # contains all the BERT extensions and baseline source code
├── Mistral/ # contains all the Mistral extensions, requirements and baseline source code
```
