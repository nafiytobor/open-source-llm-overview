# DeepSeek Model Series

![DeepSeek Logo](../../assets/images/models/deepseek-logo.png)

DeepSeek is a series of advanced large language models developed by DeepSeek AI. The series spans from lightweight models suitable for edge devices to massive models designed for cutting-edge research and enterprise applications.

## Model Versions Overview

| Model | Release Date | Parameter Size | Activation Parameters | Key Features |
|:------|:-------------|:---------------|:---------------------|:-------------|
| **DeepSeek-V3** | 2024 | 671B | 37B | Latest generation with advanced reasoning capabilities |
| **DeepSeek-V2** | 2023 | 236B | 21B | Enhanced context handling and instruction following |
| **DeepSeek-V2-Lite** | 2023 | 15.7B | 2.4B | Optimized for efficiency while maintaining strong capabilities |
| **DeepSeek 67B** | 2023 | 67B | 67B | High-capacity model for complex reasoning and generation |
| **DeepSeek 7B** | 2022 | 7B | 7B | Balanced performance for general-purpose applications |
| **DeepSeek 1.3B** | 2022 | 1.3B | 1.3B | Lightweight model for constrained environments |

## Hardware Requirements

| Model | Parameter Size | Activation Parameters | Precision | VRAM Required | System RAM Required |
|:------|:---------------|:----------------------|:----------|:--------------|:--------------------|
| **DeepSeek-V3** | 671B | 37B | FP16 | ~74 GB | ~148 GB |
| **DeepSeek-V2** | 236B | 21B | FP16 | ~42 GB | ~84 GB |
| **DeepSeek-V2-Lite** | 15.7B | 2.4B | FP16 | ~4.8 GB | ~9.6 GB |
| **DeepSeek 67B** | 67B | 67B | FP16 | ~134 GB | ~268 GB |
| **DeepSeek 7B** | 7B | 7B | FP16 | ~14 GB | ~28 GB |
| **DeepSeek 1.3B** | 1.3B | 1.3B | FP16 | ~2.6 GB | ~5.2 GB |

## Model Architecture

DeepSeek models are based on the transformer architecture with several key innovations:

- **Mixture of Experts (MoE)**: DeepSeek-V2 and V3 utilize MoE architecture to achieve significantly higher effective parameter counts while keeping compute requirements manageable
- **Advanced Activations**: Specialized activation functions for improved training stability and inference quality
- **Efficient Attention Mechanisms**: Modified attention mechanisms to better handle long-range dependencies
- **Optimized Training Methodology**: Custom pre-training curricula and fine-tuning approaches

## Performance Benchmarks
tbd