---
title: Image Restoration
categories:
- General
excerpt: |
  Enhanced images' detail by restoring sharp details and clarity, making them look clean and high-resolution.

permalink: /image-restoration/
---

### Introduction
Implemented a real-time image restoration pipeline to enhance images quailty by generating high-frequency details. The system is based on DiffBIR, which restores sharp, de-noised images while preserving structure and content. The project focused on optimizing the model for deployment using quantization and lightweight inference NCNN and Vulkan, enabling efficient inference in resource-limit environment.

### Key Contributions
- Enhanced fine details in images with targeted face refinement.
- Mitigated hallucination artifacts of human faces by cropping face region—to guide the model in generating realistic facial details.
- Seamlessly blended the face-enhanced output into the full image for natural and visually consistent results.
- Optimized a heavy image restoration model to run on limited hardware.
  - Compressed input data by half with minimal quality loss
  - Quantized model weights
  - Enabled to deploy on GPUs with 50% less memory without significant performance degradation.

#### Skills
- Languages: Python
- ML Framework: Pytorch
- Optimization: Quantization
- Libraries & Tools: OpenCV, NCNN, Vulkan, Docker