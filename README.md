# BFSI LLM Chatbot — Flan-T5-Large with Few-Shot Prompt Engineering

MSc Data Science Dissertation — Liverpool John Moores University, 2025  
**Author:** Srijan Kumar Awasthi

## Overview
Evaluation of zero-cost few-shot prompt engineering for adapting 
Flan-T5-Large to BFSI retail banking customer service queries.
Compares a zero-shot baseline (Condition A) against a structured 
few-shot BFSI system prompt (Condition B) across quantitative 
metrics and red-team adversarial evaluation.

## Key Results
- 70% reduction in hallucination rate (7.69% → 2.31%)
- 24% improvement in perplexity (125.18 → 94.65)
- 53% improvement in ROUGE-L (0.069 → 0.106)
- Red-team avg quality score: 3.94 / 5.0 (few-shot)

## Datasets
**Primary — Bitext Retail Banking LLM Chatbot Training Dataset**  
26,872 intent-labelled retail banking queries (CC BY 4.0)  
https://huggingface.co/datasets/bitext/Bitext-retail-banking-llm-chatbot-training-dataset

**Secondary — LMSYS Chatbot Arena Conversations**  
~2,000 curated single-turn exchanges for qualitative evaluation  
https://huggingface.co/datasets/lmsys/chatbot_arena_conversations

## Model
Flan-T5-Large (google/flan-t5-large) — Apache 2.0  
https://huggingface.co/google/flan-t5-large

## Requirements
Python 3.10+
transformers
scikit-learn
pandas
numpy
rouge-score
sacrebleu
datasets
torch
