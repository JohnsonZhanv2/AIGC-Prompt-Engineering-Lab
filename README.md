# 🔬 AIGC Prompt Engineering & Latent Diffusion Lab

This repository documents my research and optimization process for **Stable Diffusion (WebUI)**. As an Electronic Engineering student at HKU, I focus on the mathematical convergence of samplers and the precision of image reconstruction.

## 🚀 Lab Contents
- **[SD_WebUI_Lab.ipynb](./SD_WebUI_Lab.ipynb)**: Core environment setup for Google Colab (Tesla T4).
- **[Prompts Library](./prompts.txt)**: A collection of high-performing prompt templates for Cyberpunk, Underwater, and Material Physics styles.
- **[Optimization Logs](./webui_config.png)**: Visual records of parameter tuning.

## 🛠️ Technical Deep Dive

### 1. Sampler Analysis: DPM++ 2M SDE Karras
Compared to Euler a, this second-order stochastic differential equation solver provides:
- **Higher Fidelity**: Sharper micro-details in hair and eye iris textures.
- **Stable Convergence**: Reduced artifacts during the denoising process between 25-35 steps.

### 2. Reconstruction Logic (Hires. fix)
- **Upscaler**: R-ESRGAN 4x+ Anime6B (Optimized for edge sharping in anime-style illustrations).
- **Denoising strength**: Maintained at **0.45** to ensure structural consistency while enhancing pixel density.

## 🖼️ Featured Results
| Style | Preview | Key Parameters |
| :--- | :---: | :--- |
| **Cyberpunk** | ![Cyber](./cyber_sample.png) | CFG 7, Steps 28, Vivid Colors |
| **Material Physics** | ![Material](./material_sample.png) | Buttons straining, 0.55 Denoising |

---
## 🎓 About the Researcher
**Johnson Zhan** The University of Hong Kong (HKU) | Electronic Engineering
