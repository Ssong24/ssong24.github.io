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

<!-- more -->

🧠 Applied clustering and optimized rendering using mvs-texturing

👁️ Selected best views per cluster using vertex visibility analysis

🎨 Preserved vertex color data during mesh partitioning

📐 Added control over partitioning via plane size parameter

🌅 Enhanced image quality with exposure fusion, histogram equalization & reflection removal

✂️ Reduced seam artifacts by refining mesh edges and fixing indoor wall textures

🚫 Removed floor projection errors using segmentation techniques

🧩 Implemented quadratic mesh simplification for performance

🔄 Generated artificial perspective views from panoramas

⚙️ Ported Python pitch/yaw projection logic to efficient C++

🪟 Merged multiple patch views by selecting visible candidates

📦 Supported testing & deployed to the production server

### Skills & Technologies

3D Geometry & Mesh Processing: mesh simplification, partitioning, vertex visibility, seam correction

Photogrammetry Tools: mvs-texturing, perspective projection

Image Processing: exposure fusion, AHE, reflection removal, segmentation

Programming Languages: Python, C++

Optimization & Performance: view selection, C++ migration for speed

Deployment: production deployment & testing support