# Overview

**Translation invariance** is an important property of **Convolutional Neural Networks (CNNs)**, especially in image processing and other grid-like data.
## Basic Concept

- A system is **translation invariant** if the **output does not change (or changes very little)** when an object in the input **shifts its position**.
- In other words, a **CNN can recognize the same feature even if it appears at different locations in the image**.
## Why CNNs Have Translation Invariance

Main mechanisms:
1. **Convolution + Parameter Sharing**
- Filters (kernels) **share weights across the whole image**.
- Each filter scans the entire image → detects the feature wherever it appears.

2. **Pooling (Max/Average Pooling)**
- Reduces the spatial size of feature maps, making the network **less sensitive to small shifts**.
- Example: Max pooling over 2×2 regions → exact feature location becomes less important.

3. **Data Augmentation (during training)**
- Shift, rotate, flip images → network learns to recognize features regardless of position or small transformations.
# Links
## Articles
- [All you should know about translation equivariance/invariance in CNN | by Sue | Medium](https://medium.com/@sue.sk.guo/all-you-should-know-about-translation-equivariance-invariance-in-cnn-cbf2a2ad33cd)
- [A Friendly Introduction to Convolutional Neural Networks | Hashrocket](https://hashrocket.com/blog/posts/a-friendly-introduction-to-convolutional-neural-networks)
## Videos
- [(40) 05 Imperial's Deep learning course: Equivariance and Invariance - YouTube](https://www.youtube.com/watch?v=a4Quhf9NhMY)
## Papers
- [[2103.10097] Stride and Translation Invariance in CNNs](https://arxiv.org/abs/2103.10097)