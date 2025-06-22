---
title: Object Detector with Fisheye Images
categories:
- Machine Learning 
excerpt: |
  Improved Object detection accuracy by applying an extended projection method based on spherical projection for fisheye lenses, incorporating an expansion coefficient to interpolate pixel values of distorted objects

permalink: /obj-det-fisheye/
---



#### Abstract
Accurate object detection from wide-angle views is essential for advanced autonomous driving. Fisheye lens cameras are useful in this context but introduce heavy radial distortion — objects in the center appear larger, while those near the edges look smaller.
To address this, we propose Expandable Spherical Projection, which selectively expands the center or edge regions of fisheye images. This helps straighten object edges and reduce background noise in bounding boxes.
We also explore multi-scale feature fusion in real-time object detection using three variations of a YOLOv3-SPP architecture, designed to better detect small objects.

{% include button.html text="Thesis" icon="link" link="https://www.mdpi.com/2076-3417/12/5/2403" color="#000000" %}  {% include button.html text="Code" icon="github" link="https://github.com/Ssong24/Expandable-Spherical-Projection" color="#000000" %} 


#### Detection Result
![object-detection-result]({{ site.baseurl }}/assets/fisheye-lens-result.png)


#### Proposed Model Structures
![model-structures]({{ site.baseurl }}/assets/model-structure.png)


####  Demo

<video width="640" height="360" controls>
  <source src="/assets/videos/media1.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>



#### Key Contribution
- Improved object detection accuracy by 4.7% compared to models trained on uncorrected fisheye images
- Enabled detection inference with real-time distortion correction.
- Evaluated the impact of feature fusion structures on detection accuracy, with a focus on small object performance


#### Skills
- Language: C++
- Libraries: OpenCV



