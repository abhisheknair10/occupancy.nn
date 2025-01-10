# Occupancy.nn - Train and Inference Occupancy Networks

<div align="center">
  <img src="https://github.com/abhisheknair10/occupancy.nn/blob/main/assets/3d-reconstruction.jpg" alt="inference" width="600">
</div>

> This project is a work in progress (early stages), but is being actively developed.

# Introduction

### *Current State of 3D Reconstruction from Vision*

Reconstructing a 3D scene is a non-trivial task and can be done in a lot of ways:

- Stereo Vision is a traditional method that uses geometry to figure out depth information by comparing points and features across an image. 

- On the other hand, deep learning techniques like NeRFs and Gaussian Splatting are newer, data-driven methods. These approaches use a set of images of a scene taken from different angles to train a model that can represent the scene. With good-quality data, deep learning techniques are usually more accurate and easier to work with.

But there’s a catch. Techniques like NeRFs and Gaussian Splatting are offline methods. You need to have all the images of the scene beforehand, train the model, and only then can you get depth information. This makes them unsuitable for real-time applications like Tesla Vision, where the system needs to reconstruct the scene in real-time to make real-time decisions based on scene and environment semantics.

### *Realtime Methods*

Voxel-based methods provide another approach, allowing models to predict density at discrete points in a 3D grid. However, this approach has a major limitation: resolution. Since the grid is discrete, the resolution at which the scene can be reconstructed is restricted by memory and computational limits.

This is where Occupancy Networks step in:

- They utilize their understanding of scene semantics to represent the scene as a continuous function, rather than a discrete grid.

- This means you can query any specific point in the scene to determine the probability that it is occupied, enabling high-resolution reconstructions without being limited by grid size.

Occupancy Networks bridge the gap between offline accuracy and real-time flexibility, making them a powerful choice for scene reconstruction tasks.

# Occupancy Networks

<div align="center">
  <img src="https://github.com/abhisheknair10/occupancy.nn/blob/main/assets/occupancy.jpg" alt="inference" width="600">
</div>

> Building stuff right now. Nothing to see here yet.