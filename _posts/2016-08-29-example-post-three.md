---
title: Visual Object Tracking with Pivo Pod
categories:
- General
excerpt: |
  Group two racket players from detected bounding boxes and track the box using Pivo pod.
feature_text: |
  ## Group Tracking
  This feature is designed to detect the racket player, smoothing capture the solo or pair training.
feature_image: "/assets/premium_photo-1666913667023-4bfd0f6cff0a.avif"
image: "https://picsum.photos/2560/600?image=733"
---

![tracking_img]({{ site.baseurl }}/assets/full-shot-women-playing-paddle-tennis.webp)

Group two racket players from detected bounding boxes and track the box using Pivo pod. Given the racket players video, we train detector of person and racket, and select most suitable two people using previous box, confidence and size of the bounding box info. Optimize the inference and implement on mobile device. 


#### Achievements
 - Train model 
 - Applied sorting to select most suitable targets among detection results
 - Trained and evaluated racket player custom dataset
 - Detector Model compression and optimization for real-time inference in mobile device
