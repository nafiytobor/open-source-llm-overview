# NVIDIA Project DIGITS

![NVIDIA Project DIGITS](../../assets/images/hardwares/nvidia-project-digits-logo.jpg)

NVIDIA Project DIGITS is a cutting-edge portable AI system designed for high-performance edge computing. Powered by the NVIDIA GB10 Grace Blackwell Superchip, it delivers data center-class AI performance in a portable form factor.

## Specifications

<div class="spec-grid">
  <div class="spec-card">
    <div class="spec-title">System on Chip</div>
    <div class="spec-value">NVIDIA GB10 Grace Blackwell Superchip</div>
  </div>
  
  <div class="spec-card">
    <div class="spec-title">GPU</div>
    <div class="spec-value">NVIDIA Blackwell</div>
  </div>
  
  <div class="spec-card">
    <div class="spec-title">CPU</div>
    <div class="spec-value">20-core Arm®</div>
  </div>
  
  <div class="spec-card">
    <div class="spec-title">AI Performance</div>
    <div class="spec-value">1 PFLOP FP4</div>
    <div class="spec-subtext">Equivalent to approximately 4x RTX 4090s</div>
  </div>
  
  <div class="spec-card">
    <div class="spec-title">Memory</div>
    <div class="spec-value">128 GB LPDDR5x</div>
    <div class="spec-subtext">Coherent unified system memory</div>
  </div>
  
  <div class="spec-card">
    <div class="spec-title">Connectivity</div>
    <div class="spec-value">4x USB4 Type C, Bluetooth</div>
  </div>
  
  <div class="spec-card">
    <div class="spec-title">Networking</div>
    <div class="spec-value">ConnectX, Wi-Fi, Ethernet</div>
  </div>
  
  <div class="spec-card">
    <div class="spec-title">Storage</div>
    <div class="spec-value">Up to 4 TB NVMe M.2</div>
    <div class="spec-subtext">With self-encryption</div>
  </div>
  
  <div class="spec-card">
    <div class="spec-title">Display Output</div>
    <div class="spec-value">1x HDMI 2.1a</div>
  </div>
  
  <div class="spec-card">
    <div class="spec-title">Power</div>
    <div class="spec-value">Standard wall outlet</div>
  </div>
  
  <div class="spec-card">
    <div class="spec-title">Operating System</div>
    <div class="spec-value">NVIDIA DGX™ Base OS, Ubuntu Linux</div>
  </div>
</div>

## LLM Compatibility

Project DIGITS can run a wide range of open-source LLMs, including:

<div class="model-badges">
  <span class="model-badge llama">LLaMA 3 8B</span>
  <span class="model-badge llama">LLaMA 2 7B</span>
  <span class="model-badge llama">LLaMA 2 13B</span>
  <span class="model-badge mistral">Mistral 7B</span>
  <span class="model-badge gemma">Gemma 7B</span>
  <span class="model-badge gemma">Gemma 2B</span>
</div>

With appropriate quantization, it can also run larger models like:

<div class="model-badges">
  <span class="model-badge llama">LLaMA 3 70B (Quantized)</span>
  <span class="model-badge llama">LLaMA 2 70B (Quantized)</span>
</div>

## Key Features

### Unified Memory Architecture

The Project DIGITS system features a unified memory architecture that allows the CPU and GPU to access the same physical memory, eliminating costly data transfers between separate memory pools. This architecture is particularly beneficial for LLM inference, where model weights need to be accessed by both the CPU and GPU.

### Portable Form Factor

Despite its impressive performance capabilities, Project DIGITS comes in a portable form factor that can be easily transported, making it ideal for:

- Field research
- On-site AI demonstrations
- Mobile development workstations
- Edge deployment scenarios

### Enterprise-Grade Security

With built-in self-encrypting storage and advanced security features from the NVIDIA DGX Base OS, Project DIGITS is designed with enterprise-grade security in mind, making it suitable for handling sensitive data and models.

### Development Environment

Project DIGITS comes with a full Ubuntu Linux-based operating system, providing a familiar and powerful development environment with access to:

- CUDA and TensorRT
- Popular AI frameworks like PyTorch and TensorFlow
- Triton Inference Server
- NVIDIA AI Enterprise software stack

## Use Cases

### On-Device LLM Inference

Project DIGITS is ideal for running LLM inference workloads locally, with sufficient performance to run multiple 7B-13B parameter models simultaneously. This makes it perfect for:

- Private AI deployment where data cannot leave the device
- Offline AI capabilities in disconnected environments
- Low-latency AI applications

### AI Research and Development

The combination of powerful hardware and a full development environment makes Project DIGITS an excellent platform for AI research and development, supporting:

- Model fine-tuning
- Prompt engineering
- Application development and testing
- Experimentation with multiple models

### Edge AI Deployment

For organizations looking to deploy AI at the edge without the limitations of traditional edge devices, Project DIGITS offers data center-class performance in a portable package, enabling:

- On-site natural language processing
- Local computer vision applications
- Edge analytics with AI assistance