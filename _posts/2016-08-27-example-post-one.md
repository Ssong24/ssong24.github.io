---
title: 3D Mesh Texturing
categories:
- General
- External sources
excerpt: |
  Textured 3D indoor reconstructions by partitioning input meshes into planes and mapping optimal camera views based on vertex visibility and clustering.
feature_image: "/assets/3d-mesh-texture.png"
---

Textures 3D reconstructions of indoor scenes from 2D images and camera poses.  Given as input a mesh(.ply) and camera poses, apply partitioning the mesh into planes and rendering the model under given poses, and generates vertex visibility data per frame. Based on partition result a cluster-plane index files and vertex visibility, generate texture patch by mapping each clustered plane with one camera view. 


### Key Achievements
🧠 Applied clustering and optimized rendering using mvs-texturing
🌅 Enhanced image quality with exposure fusion, histogram equalization and reflection removal
✂️ Reduced seam artifacts by refining mesh edges and fixing indoor wall textures
🧩 Implemented quadratic mesh simplification for performance
🔄 Generated artificial perspective views from panoramas
📦 Supported testing & deployed to the production server

### Skills & Technologies
- 3D Geometry & Mesh Processing: mesh simplification, partitioning, vertex visibility, seam correction
- Photogrammetry Tools: mvs-texturing, perspective projection
- Image Processing: exposure fusion, AHE, reflection removal, segmentation
- Programming Languages: Python, C++
- Deployment: Docker