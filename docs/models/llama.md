# LLaMA Model Series

![LLaMA Logo](../../assets/images/llama-logo.png)

LLaMA (Large Language Model Meta AI) is a series of open-source large language models developed by Meta AI.

## Model Versions

### LLaMA 3

| Model Name | Parameters | Context Length | Quantized Versions | Release Date | Training Data |
|------------|------------|----------------|-------------------|--------------|--------------|
| LLaMA 3 8B | 8B | 8K | GGUF (Q4_K_M) | April 2024 | 15T tokens |
| LLaMA 3 70B | 70B | 8K | GGUF (Q4_K_M) | April 2024 | 15T tokens |

### LLaMA 2

| Model Name | Parameters | Context Length | Quantized Versions | Release Date | Training Data |
|------------|------------|----------------|-------------------|--------------|--------------|
| LLaMA 2 7B | 7B | 4K | GGUF (Q4_K_M) | July 2023 | 2T tokens |
| LLaMA 2 13B | 13B | 4K | GGUF (Q4_K_M) | July 2023 | 2T tokens |
| LLaMA 2 70B | 70B | 4K | GGUF (Q4_K_M) | July 2023 | 2T tokens |

## Performance Metrics

### General Capability Tests

<div class="chart-container">
    <canvas id="llama-general-benchmark"></canvas>
</div>

| Benchmark | LLaMA 3 8B | LLaMA 3 70B | LLaMA 2 7B | LLaMA 2 13B | LLaMA 2 70B |
|-----------|------------|------------|------------|-------------|-------------|
| MMLU | 64.2% | 79.5% | 46.9% | 54.8% | 68.9% |
| HumanEval | 42.7% | 67.2% | 23.7% | 29.8% | 37.5% |
| GSM8K | 71.3% | 87.8% | 28.7% | 36.8% | 63.2% |

### Specialized Task Performance

<div class="chart-container">
    <canvas id="llama-specialized-tasks"></canvas>
</div>

## Architectural Features

LLaMA 3 employs an improved Transformer architecture with key innovations including:

- Optimized attention mechanisms
- Enhanced positional encoding
- Improved training methods and data processing

## Deployment Requirements

| Model Version | Min VRAM (FP16) | Recommended VRAM (Quantized) | CPU Memory Requirements |
|---------------|-----------------|------------------------------|-------------------------|
| LLaMA 3 8B | 16GB | 8GB (Q4_K_M) | 16GB |
| LLaMA 3 70B | 140GB | 40GB (Q4_K_M) | 64GB |

## Usage Example

```python
from transformers import AutoModelForCausalLM, AutoTokenizer

# Load model and tokenizer
model_name = "meta-llama/Llama-3-8B"
tokenizer = AutoTokenizer.from_pretrained(model_name)
model = AutoModelForCausalLM.from_pretrained(model_name)

# Generate text
input_text = "Explain the basic principles of quantum computing:"
inputs = tokenizer(input_text, return_tensors="pt")
outputs = model.generate(**inputs, max_length=200)
result = tokenizer.decode(outputs[0], skip_special_tokens=True)
print(result)