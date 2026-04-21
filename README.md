# Receiver Inference in Relational Event History Data  
## Reconstructing Communication Networks with Large Language Models

This repository contains the code accompanying the paper:

> *Receiver Inference in Relational Event History Data: Reconstructing Communication Networks with Large Language Models*

The project focuses on inferring **message addressees (receivers)** in multi-party conversations—specifically parliamentary debates—using large language models (LLMs), and evaluating the resulting communication networks.

---

## Overview

Relational Event History (REH) datasets often include information about **who speaks**, but lack explicit information about **who is being addressed**. This repository provides a framework to:

- Infer receivers using an API  
- Construct directed communication networks  
- Evaluate predictions at both the **turn level** and **network level**  
- Analyze model confidence and uncertainty  

The implementation is applied to Dutch parliamentary debate transcripts.

---

## Repository Structure

```text
├── prompts/                           # Few-shot prompt templates
├── src/
│   ├── inference.py                   # API calls for receiver prediction
│   ├── turn_level_evaluation.py       # Turn-level evaluation metrics
│   ├── network_level_evaluation.py    # Network construction and analysis
│   ├── statistics.py                  # Calculated statistics, self-assessed confidence scores and logprob analysis 
│   ├── rem_analysis.py                # Relational event analysis
└── README.md
