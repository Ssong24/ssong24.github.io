---
title: Object Detection with Fisheye Lens Image
categories:
- General
excerpt: |
  Improved Object detection accuracy by applying an extended projection method based on spherical projection for fisheye lenses, incorporating an expansion coefficient to interpolate pixel values of distorted objects

permalink: /obj-det-fisheye/
feature_image: "/assets/premium_photo-1666913667023-4bfd0f6cff0a.avif"
image: "https://picsum.photos/2560/600?image=733"
---

{% include button.html text="Code" icon="github" link="https://github.com/Ssong24/Expandable-Spherical-Projection" color="#000000" %} 

## Abstract
Accurate object detection from wide-angle views is essential for advanced autonomous driving. Fisheye lens cameras are useful in this context but introduce heavy radial distortion — objects in the center appear larger, while those near the edges look smaller.

To address this, we propose Expandable Spherical Projection, which selectively expands the center or edge regions of fisheye images. This helps straighten object edges and reduce background noise in bounding boxes.

We also explore multi-scale feature fusion in real-time object detection using three variations of a YOLOv3-SPP architecture, designed to better detect small objects.

#### Object Detection Result from Fisheye images
![object-detection-result]({{ site.baseurl }}/assets/fisheye-lens-result.png)


#### Proposed Three types of Feature concatenation YOLOv3-SPP Model Structure
![model-structures]({{ site.baseurl }}/assets/model-structure.png)


<video width="640" height="360" controls>
  <source src="/assets/media1.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>



#### Key Contribution
● Improved object detection accuracy by 4.7% compared to models trained on uncorrected fisheye images
● Enabled detection inference with real-time distortion correction.
● Evaluated the impact of feature fusion structures on detection accuracy, with a focus on small object performance


#### Skills
- Language: C++, Python
- ML Framework: Pytorch
- Base model: YOLOv3
- Dataset: 
    - Custom Fisheye Dataset ([Fisheye-Dongseongro](https://github.com/Ssong24/Fisheye-Dongseongro)), 
    - Systhetic Fisheye Dataset from: [KITTI](https://www.cvlibs.net/datasets/kitti/eval_object.php?obj_benchmark=2d), [CityScapes](https://www.cityscapes-dataset.com/)



