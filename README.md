# Occupancy.nn - Pipeline to Train and Inference Occupancy Networks

> This project is a work in progress, but is being actively developed.

# Introduction

Reconstructing a 3D scene is a non-trivial task that can be performed using multiple styles and techniques. Stereo Vision is a geometric technique to extract/calculate depth information of different points and features across an image. Deep Learning based techniques, like NeRFs and Gaussian Splatting, are popular data driven techniques allowing a sparse set of images of a scene from varying perspectives, to optimize a model to implicitly represent the scene. Deep Learning techniques tend to perform much better and are much easier to train, as long as good quality data is attainable.

However, to get depth information of a view in a scene, NeRFs and Gaussian Splatting are offline deep learning techniques, which means that the entire set of images of the scene have to be acquired, train a model, and then only can you get dfepth information. Such techniques wont be possible for realtime use cases liek Tesla Vision, which reconstructs a scene in realtime to understand scene presence and enviuronemtn semantics.

Reconstructing a 3D scene is a non-trivial task and can be done in a lot of ways. 

Stereo Vision is a traditional method that uses geometry to figure out depth information by comparing points and features across an image. 

On the other hand, deep learning techniques like NeRFs and Gaussian Splatting are newer, data-driven methods. These approaches use a set of images of a scene taken from different angles to train a model that can represent the scene. With good-quality data, deep learning techniques are usually more accurate and easier to work with.

But there’s a catch. Techniques like NeRFs and Gaussian Splatting are offline methods. You need to have all the images of the scene beforehand, train the model, and only then can you get depth information. This makes them unsuitable for real-time applications like Tesla Vision, where the system needs to reconstruct the scene in real-time to make realtime decisions based on scene and environment semantics.

This is where occupancy networks come in.

# Occupancy Networks

> Building stuff right now. Nothing to see here yet.