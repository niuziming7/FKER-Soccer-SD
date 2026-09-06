# FKER: Football Knowledge-Enhanced Reasoning for Chinese Soccer Stance Detection

This repository contains reproducibility materials for the paper:

> 基于知识增强推理的足球社交领域立场检测

## Overview

FKER constructs sample-level football background knowledge from fan-identity cues, metaphor-to-entity mappings, and fan-relation graphs. It further performs structured reasoning for target entity extraction and stance detection.

## Released Materials

The current release includes:

- Prompt templates for Gemini-3.0-Flash controlled experiments;
- Gemini API configuration and inference settings;
- Results of Gemini direct prompting, +CoT, +KB, and +KB+CoT;
- Evaluation protocol and output normalization rules.

The Soccer-SD dataset, football knowledge base, data processing code, training and inference scripts, and LoRA adapter weights will be released upon formal publication, subject to relevant data-use requirements.

## Gemini Controlled Results

| Setting | Target Acc (%) | Stance F1 (%) | Joint Acc (%) |
|---|---:|---:|---:|
| Gemini-3.0-Flash | 47.13 | 52.18 | 39.10 |
| Gemini-3.0-Flash + CoT | 48.09 | 53.77 | 41.24 |
| Gemini-3.0-Flash + KB | 50.64 | 54.24 | 43.33 |
| Gemini-3.0-Flash + KB + CoT | 52.77 | 56.21 | 47.78 |

## Repository Structure

```text
prompts/       Prompt templates
configs/       API and inference configurations
results/       Experimental results
evaluation/    Evaluation protocol
