# Mistral Model Series

![Mistral Logo](../../assets/images/models/mistral-logo.png)

Mistral is a series of advanced large language models developed by Mistral AI. The series features a range of models from efficient base models to specialized variants for specific domains like code and mathematics, as well as mixture-of-experts architectures that offer significant performance improvements.

## Model Versions Overview

| Model | Release Date | Parameter Size | Key Features | Input Modalities | Output Modalities |
|:------|:-------------|:---------------|:-------------|:-----------------|:------------------|
| **Mistral Small** | January 2025 | 24B | Latency-optimized, competitive with larger models, Apache2 license | Text | Text |
| **Pixtral** | September 2024 | 12B | Multimodal (text and image), Apache2 license | Text, Image | Text |
| **Mistral Nemo** | July 2024 | 12B | Large context window (128k tokens), state-of-the-art in reasoning, Apache2 license | Text | Text |
| **Codestral Mamba** | July 2024 | 7B | Specialized in code generation, Mamba architecture, Apache2 license | Text | Text |
| **Mathstral** | July 2024 | 7B | Specialized in mathematical reasoning and scientific discovery, Apache2 license | Text | Text |
| **Mixtral 8x22B** | April 2024 | 141B (8 experts of 22B each) | Sparse Mixture of Experts (SMoE), 39B active parameters, high performance-to-cost ratio, Apache2 license | Text | Text |
| **Mixtral 8x7B** | March 2024 | 56B (8 experts of 7B each) | Mixture of experts (MoE) model, efficient scaling, strong code generation, Apache2 license | Text | Text |
| **Mistral 7B** | September 2023 | 7B | Initial model, powerful for its size, efficient, Apache2 license | Text | Text |

## Hardware Requirements

| Model | Parameter Size | Activation Parameters | Precision | VRAM Required | System RAM Required |
|:------|:---------------|:----------------------|:----------|:--------------|:--------------------|
| **Mistral Small** | 24B | 24B | FP16 | ~48 GB | ~96 GB |
| **Pixtral** | 12B | 12B | FP16 | ~24 GB | ~48 GB |
| **Mistral Nemo** | 12B | 12B | FP16 | ~24 GB | ~48 GB |
| **Codestral Mamba** | 7B | 7B | FP16 | ~14 GB | ~28 GB |
| **Mathstral** | 7B | 7B | FP16 | ~14 GB | ~28 GB |
| **Mixtral 8x22B** | 141B | 39B | FP16 | ~78 GB | ~156 GB |
| **Mixtral 8x7B** | 56B | 13B | FP16 | ~26 GB | ~52 GB |
| **Mistral 7B** | 7B | 7B | FP16 | ~14 GB | ~28 GB |

## Model Architecture

Mistral models utilize several innovative architectural approaches:

- **Sliding Window Attention**: Efficient processing of longer contexts without quadratic scaling issues
- **Mixture of Experts (MoE)**: Used in Mixtral models to achieve significantly higher effective parameter counts while keeping compute requirements manageable
- **Grouped-Query Attention (GQA)**: Faster inference while maintaining model quality
- **Mamba Architecture**: State space models used in Codestral Mamba for efficient sequence modeling
- **Apache 2.0 License**: All models are available under the permissive Apache 2.0 license, allowing for commercial use

## Performance Benchmarks
tbd