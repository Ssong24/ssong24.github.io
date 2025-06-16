---
title: Pivo Object & Group Tracking Pod
categories:
- General
excerpt: |
  Developed a real-time object and group tracking system for Pivo, enabling smooth single and dual-player tracking using deep learning and mobile optimization.

permalink: /pivo-tracking/
feature_image: "/assets/premium_photo-1666913667023-4bfd0f6cff0a.avif"
image: "https://picsum.photos/2560/600?image=733"
---

![tracking_img]({{ site.baseurl }}/assets/full-shot-women-playing-paddle-tennis.webp)

## Visual Object Tracking
Contributed to enhancing the Pivo object tracking system, built on the DeepSort framework with person detection and feature extraction for Person Re-ID. Focused on improving tracking robustness and real-time performance. Current work includes optimizing the pipeline for mobile deployment through model compression techniques such as quantization, pruning, and lightweight inference for mobile device maintaining high accuracy evaluated on the test videos.

## Group Tracking
Developed a system to track two racket players simultaneously (“Double Match” feature). Built a custom detector for people and rackets, applied bounding box analysis (confidence, size, previous location) to select the most relevant two players, and implemented group tracking using the Pivo pod. Optimized the model for real-time inference on mobile devices.


#### Key Contribution
- Integrated face tracking module using AdaFace and ArcFace loss (in progress)
- Trained and evaluated a custom dataset for racket players
- Applied efficient model compression for mobile inference
- Designed selection logic for multi-player tracking based on detection attributes


{% include button.html text="Demo" icon="youtube" link="https://www.youtube.com/watch?v=jGfMteI-SVg" color="#000000" %} 

#### Demo video
[Watch on YouTube](https://www.youtube.com/watch?v=jGfMteI-SVg)

#### Skills
Pytorch, Vulkan, Kubeflow, C++